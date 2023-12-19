# Chat with Multiple PDFs



This is a Streamlit web application that allows users to chat with a conversational model trained on a set of documents/PDFs. The conversation is based on a conversational retrieval model and is designed to help users obtain information from the provided documents.

Features
Document Processing: Users can upload multiple PDF files, and the application will extract text from these files.

Conversational AI: Users can ask questions about the documents, and the application uses a conversational retrieval model to provide relevant answers based on the content of the documents.

## Steps:
## Clone the Repository:
git clone https://github.com/your_username/your_repository.git
cd your_repository

## Install Dependencies:
pip install -r requirements.txt

## Set Up Hugging Face API Token:
## Obtain your Hugging Face API key and set it as an environment variable:
export HUGGINGFACEHUB_API_TOKEN=YOUR_API_KEY

## Run the Application:
streamlit run your_app.py

## Upload PDFs:
### Use the sidebar to upload one or more PDF files.
#### Click the "Process" button to extract text from the uploaded documents.

## Ask Questions:
### Enter your questions in the text input box.
#### The application will provide answers based on the content of the uploaded documents.

# Code Overview:
def main():
    # Entry point of the application, initializes Streamlit and handles user interactions.

def get_pdf_text(pdf_docs):
    # Extracts text from the uploaded PDF documents.

def get_text_chunk(text):
    # Splits the text into chunks for efficient processing.

def get_vector_store(text_chunks):
    # Converts text chunks into vector representations using Hugging Face embeddings
    # and stores them in a FAISS vector store.

def get_conversation_chain(vectorstore):
    # Sets up a conversational retrieval chain using a Hugging Face model and the vector store.

def handle_userinput(user_question):
    # Handles user input, updates the conversation history, and displays the conversation
    # in the Streamlit app.
## Acknowledgments:

1.This project utilizes Streamlit for the web application interface.
2.Hugging Face models and embeddings are used for natural language processing.
3.The conversational retrieval chain is built using the LangChain library.

## License:

This project is licensed under the MIT License - see the LICENSE file for details.
