# Automated Recruitment Chatbot

This project involves developing a chatbot capable of automating the recruitment process. The chatbot allows the HR department to upload multiple candidate CVs in PDF format and ask specific questions to filter out candidates based on their CVs without having to manually read each one.

## Project Structure 
    ```bash
    ├── src/
    │   ├── htmlTemplates.py        # Contains HTML templates for the chat interface
    │   └── app.py                  # Main application code
    ├── README.md
    ├── requirements.txt            # List of dependencies
    └── .env  
    ```


## Features

- Upload multiple CVs in PDF format.
- Automatically process and extract text from the uploaded PDFs.
- Split the extracted text into chunks for better searchability.
- Generate embeddings using Hugging Face's `instructor-xl` model.
- Create a vector store using FAISS for efficient document retrieval.
- Ask questions about the CVs, and the chatbot will respond based on the relevant information retrieved from the PDFs.
- Maintain conversation history using `ConversationBufferMemory` to make interactions more fluid and context-aware.

## Tech Stack

- **Streamlit**: For the web interface.
- **FAISS**: Used for vector similarity search and retrieval.
- **Langchain**: For handling conversation chains and retrieval.
- **Hugging Face's Instruct Embeddings**: To generate embeddings from text.
- **PyPDF2**: To handle PDF file processing.
- **OpenAI**: For the conversational AI model.


## Installation
To set up the project locally, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone 
    ```
2. **Navigate to the project directory :**
    ```
    cd 
    ```
3. **Install the required packages using pip:**
    ```bash
    pip install Requirements.txt
    ```

3. **Create a `.env` file and add your OpenAI API key:**
    ```
    OPENAI_API_KEY=your_openai_api_key
    ```

4. **Run the Streamlit app :**
    ```
    streamlit run app.py
    ```

