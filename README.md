# PDF Search Engine

A powerful search engine that allows users to search through PDF documents using natural language queries. This project utilizes `fitz` for PDF parsing, `AutoTokenizers` for text tokenization, and the cosine similarity for finding best chunk match. The Gemini API for advanced language model integration.

## Steps

- **PDF Parsing**: Extract text from PDF documents using `fitz`.
- **Document Chunking** : chunked extracted text in a fixed size
- **Text Tokenization and Encoding** : Used `sentence-transformers/all-MiniLM-L6-v2` to tokenize and encoding the chunks
- **Query input and Cosine similariy** : Convert the query using the same model into embddings, find cosine similairty and choose top
- **Natural Language Search**: Leveraged the Gemini API to process user queries and return relevant results.
