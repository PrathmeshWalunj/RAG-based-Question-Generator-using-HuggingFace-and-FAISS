# RAG-based-Question-Generator-using-HuggingFace-and-FAISS
This project demonstrates a Retrieval-Augmented Generation (RAG) system that generates questions from PDFs using HuggingFace models and FAISS for efficient document retrieval. The application takes 5-10 PDFs as input, extracts text, retrieves relevant sections based on user queries, and generates questions using a pre-trained HuggingFace model.
# Project Workflow
1. PDF Text Extraction:
Extract text from uploaded PDF files using the PyMuPDF library.
2. Text Embeddings Generation:
Text is split into sections and embeddings are generated using the SentenceTransformer model (all-MiniLM-L6-v2).
3. FAISS Index for Retrieval:
Embeddings are stored in a FAISS index to enable fast similarity search and retrieval of relevant sections based on user queries.
4. Question Generation:
Retrieved sections are passed to a HuggingFace T5 model (valhalla/t5-base-qg-hl) to generate questions.
# Technologies Used
1. Python for core development.
2. HuggingFace Transformers for question generation.
3. FAISS for vector-based document retrieval.
4. PyMuPDF for PDF text extraction.
5. SentenceTransformer for generating embeddings.
6. Streamlit or Gradio (optional) for building a simple UI to upload PDFs and display generated questions.
# How to Run the Project
1. Clone the repository
2. Install required libraries
3. Run the application
4. Upload your PDFs and generate questions
# Future Improvements
1. Add support for other document formats (e.g., DOCX).
2. Improve the question generation accuracy using more advanced models.
3. Allow more customization in question generation (e.g., specifying difficulty levels).
