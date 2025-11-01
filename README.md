# PDF Assistant Chatbot

A Streamlit-based web application that allows users to interact with PDF documents using AI-powered chat functionality. The application uses the Groq API for natural language processing and provides a user authentication system.

## Features

- **User Authentication**
  - Sign up with email and password
  - Login system
  - Secure user data storage in CSV format

- **PDF Processing**
  - Upload PDF documents
  - Extract text content from PDFs
  - View PDF content within the application

- **AI Chat Capabilities**
  - Ask questions about uploaded PDF content
  - Intelligent responses using Groq's LLaMA 3.1 model
  - Direct chat with the AI bot
  - Handles large PDF documents by processing them in chunks

## Prerequisites

- Python 3.x
- Required Python packages:
  - streamlit
  - pymupdf
  - pandas
  - python-dotenv
  - langchain-groq

## Setup

1. Clone the repository to your local machine.

2. Install the required dependencies:
   ```bash
   pip install streamlit pymupdf pandas python-dotenv langchain-groq
   ```

3. Create a `.env` file in the project root directory with the following contents:
   ```
   GROQ_API_KEY=your_groq_api_key_here
   ```

4. Run the application:
   ```bash
   streamlit run main.py
   ```

## Usage

1. **Sign Up/Login**
   - New users can create an account using their email and password
   - Existing users can log in with their credentials

2. **Working with PDFs**
   - Upload a PDF file using the "Upload PDF" option
   - View the extracted text content
   - Ask questions about the PDF content

3. **Chat Features**
   - Use "Ask Question" to inquire about the uploaded PDF
   - Use "Chat with Bot" for general conversation with the AI

## File Structure

- `main.py` - Main application file containing the Streamlit interface and logic
- `users.csv` - Database file storing user credentials
- `.env` - Environment variables file (needs to be created)

## Security Note

This is a basic implementation and may need additional security measures for production use. The current version stores passwords in plaintext in the CSV file, which is not recommended for production environments.

## License

[Add your license information here]

## Contributors

[Add contributor information here]