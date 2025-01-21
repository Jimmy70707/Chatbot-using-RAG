# RAG Q&A Conversation With PDF Including Chat History

This project is a Streamlit application that enables users to upload PDF documents, process their contents, and interact with them using a Conversational Retrieval-Augmented Generation (RAG) system. The application keeps a chat history for context-aware question answering.

## Features
- Upload and process PDF files.
- Use Groq API for powerful LLM-backed conversational capabilities.
- Chat with the uploaded documents leveraging embeddings and a retriever.
- Retain chat history to improve contextual understanding.

## Requirements
- Python 3.8+
- Required Python libraries:
  - `streamlit`
  - `langchain`
  - `langchain-chroma`
  - `langchain-community`
  - `langchain-core`
  - `langchain-groq`
  - `langchain-huggingface`
  - `langchain-text-splitters`
  - `python-dotenv`

## Setup

1. Clone the repository:
    ```bash
    git clone <repository-url>
    cd <repository-folder>
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Create a `.env` file in the project directory and set your Hugging Face token:
    ```
    HF_TOKEN=your_huggingface_token
    ```

4. Run the Streamlit application:
    ```bash
    streamlit run app.py
    ```

## Usage

1. Open the application in your browser (Streamlit will display the URL).

2. Enter your Groq API key.

3. Upload one or more PDF files to process their contents.

4. Ask questions about the content of the uploaded PDFs. The system will leverage context from the chat history to provide accurate and concise answers.

5. Review the chat history for better insights.

## File Structure
```
project-folder/
├── app.py                 # Main Streamlit application file
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (not included in repo)
├── docs/
│   └── chroma/            # Directory for persistent embeddings
└── temp.pdf               # Temporary storage for uploaded PDF files
```

## Key Components
- **Document Processing**: Upload and split PDFs into smaller chunks for embedding creation using Hugging Face.
- **Retriever**: Implements Chroma for document retrieval based on embeddings.
- **LLM Integration**: Uses Groq API for conversational and contextual understanding.
- **Chat History**: Preserves the chat context using `ChatMessageHistory` for better response quality.

## Environment Variables
- `HF_TOKEN`: Hugging Face API token for embedding creation.

## Future Enhancements
- Add support for additional file formats.
- Implement user authentication for secure API key storage.
- Enhance UI/UX for better interactivity.

## License
This project is licensed under the MIT License.

## Acknowledgements
- [LangChain](https://github.com/hwchase17/langchain)
- [Hugging Face](https://huggingface.co)
- [Streamlit](https://streamlit.io)
