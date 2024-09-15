# News Analysis Chatbot
This Streamlit application allows users to input URLs of news articles, processes the content, and provides intelligent answers to questions based on the articles. It uses OpenAI's language models and FAISS for efficient information retrieval.

## Features
- **Input Multiple URLs**: Enter up to three news article URLs in the sidebar.
- **Data Processing**: Loads and processes the articles to prepare them for querying.
- **Question Answering**: Ask questions related to the content of the articles, and get detailed answers with sources.

## Technologies Used
- **Streamlit**: For the web application interface.
- **LangChain**: For integrating OpenAI models and creating the retrieval-based question-answering system.
- **OpenAI**: For language model embeddings and question-answering.
- **FAISS**: For efficient similarity search on large-scale embeddings.
- **Python**: The programming language used.
  
## Installation
### 1. Clone the Repository:

```bash
git clone https://github.com/mshaadk/News-Analysis-Chatbot.git
cd News-Analysis-Chatbot
```

### 2. Create and Activate a Virtual Environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Required Packages:

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables: Create a .env file in the root directory and add your OpenAI API key:

```plaintext
OPENAI_API_KEY=your_openai_api_key
```

## Usage
### 1. Run the Streamlit App:

```bash
streamlit run app.py
```

### 2. Interact with the Application:

- **Input URLs**: Enter up to three news article URLs in the sidebar.
- **Process URLs**: Click the "Process URLs" button to load and process the articles.
- **Ask Questions**: Enter your questions in the provided text input to get answers based on the processed articles.
  
## Notes
- Make sure you have a valid OpenAI API key. Without it, the application won't be able to generate responses.
- Processing the articles may take some time depending on their length and content.
- The FAISS index is stored in `faiss_store_openai.pkl` and is loaded from this file when querying.

## Contributing
Feel free to fork the repository and submit pull requests. Please ensure that your changes are well-documented and tested.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE.txt) file for details.
