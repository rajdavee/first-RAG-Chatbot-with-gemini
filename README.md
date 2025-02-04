# First RAG Chatbot with Google Gemini

This is a Retrieval-Augmented Generation (RAG) powered chatbot built using Google's Gemini AI. The system can answer questions based on the data provided through documents. The chatbot integrates the power of Google's Gemini API to retrieve and generate answers relevant to the given data.

## Features

- **Document-based QA**: Allows users to input a document, and the system provides answers specific to the content of that document.
- **Powered by Google Gemini**: Uses Google's Gemini API for generating responses, with integration for RAG.

## Prerequisites

Before running the app, make sure you have the following:

- Python 3.7 or later
- A valid Google Gemini API key (required for generating responses using Google's Gemini models)
- Streamlit (for running the app)

## Installation

Follow these steps to set up the project:

### 1. Clone the Repository

Clone the repository to your local machine using the following command:

```bash
git clone https://github.com/rajdavee/irst-RAG-Chatbot-with-gemini.git
cd irst-RAG-Chatbot-with-gemini
```

### 2. Create a Virtual Environment (Optional but Recommended)

It's recommended to create a virtual environment to manage dependencies.

```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts ctivate
```

### 3. Install Dependencies

Install the required Python libraries using the provided `requirements.txt` file.

```bash
pip install -r requirements.txt
```

### 4. Add Environment Variables

In the root folder of the project, create a `.env` file. Add your Google Gemini API key in the `.env` file as follows:

```bash
GEMINI_API_KEY=your_gemini_api_key_here
```

Replace `your_gemini_api_key_here` with your actual Google Gemini API key. You can obtain this key by signing up for Google's API [here](https://developers.google.com/ai).

### 5. Run the Application

Run the Streamlit app using the following command:

```bash
streamlit run StreamlitApp.py
```

This will start the Streamlit app in your browser, where you can interact with the chatbot.

## Usage

- After running the Streamlit app, you can input a document and ask questions about the content of that document.
- The chatbot will retrieve relevant information from the document and generate a response using Google's Gemini models.

## Additional Notes

- Make sure to monitor your Google Gemini API usage, as the API may have usage limits or charges based on usage.
- If you need to modify the model or the response handling, you can edit the logic within `StreamlitApp.py` or the functions that handle API calls.

## License

This project is open-source and available under the [MIT License](LICENSE).
