# Implementing-RAGAS-Evaluation-Metrics
The app implements RAGAS (Robustness and Generality Assessment Suite) metrics to evaluate the quality of the generated answers. Specifically, it measures faithfulness, answer relevancy, context recall, and context precision.

This Streamlit application allows users to upload a PDF file and ask questions related to its content using OpenAI's GPT-3.5-turbo model. The application splits the PDF text into manageable chunks, embeds these chunks using OpenAI embeddings, and stores them in a FAISS vectorstore for efficient retrieval. Upon receiving a user question, the system retrieves relevant text chunks from the vectorstore and generates an answer based on the context provided.


# Ask Your PDF: Implementing RAGAS Metrics

Ask Your PDF is a Streamlit application that allows users to upload a PDF file and ask questions related to its content using OpenAI's GPT-3.5-turbo model. The application utilizes advanced text processing techniques to split the PDF content into manageable chunks, embeds these chunks using OpenAI embeddings, and stores them in a FAISS vectorstore for efficient retrieval. Users can input questions about the PDF, and the system generates answers based on the context derived from the stored text chunks.

Additionally, the app incorporates RAGAS (Robustness and Generality Assessment Suite) metrics to evaluate the quality of the generated answers. These metrics include:
- **Faithfulness**: Determines how accurately the answer reflects the information in the PDF.
- **Answer Relevancy**: Evaluates the relevance of the generated answer to the user's question.
- **Context Recall**: Measures how well the app recalls and uses relevant context from the PDF.
- **Context Precision**: Assesses the precision of the context provided in generating the answer.

## Key Features
- **PDF Upload**: Users can upload any PDF file to the app.
- **Text Extraction and Splitting**: The app extracts text from the PDF and splits it into chunks for efficient processing.
- **Vectorstore**: Text chunks are embedded and stored in a FAISS vectorstore for quick retrieval.
- **Question Answering**: Users can ask questions related to the content of the uploaded PDF, and the app generates answers using the retrieved text chunks.
- **RAGAS Metrics Evaluation**: The app evaluates the generated answers using predefined ground truths and displays the results in a structured manner.

## How to Use
1. **Enter OpenAI API Key**: Input your OpenAI API key to enable the model's functionality.
2. **Upload PDF**: Upload the PDF file you want to query.
3. **Ask a Question**: Enter a question related to the content of the uploaded PDF.
4. **View Answers and Evaluation**: The app will display the generated answer and evaluate its quality using RAGAS metrics.

5. I've included a section under "Notebooks" that links to the `test.ipynb` notebook located in the `Notebooks` folder. This provides with an example of how to utilize the Ask Your PDF functionality within a Jupyter notebook environment. Adjustments can be made to the paths and details based on the actual structure of your project.


## Installation
To run this application locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ask-your-pdf.git

