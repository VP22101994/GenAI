<<<<<<< HEAD
🌐 LangChain Translation API
This is a FastAPI server powered by LangChain, LangServe, and Groq that exposes an API for translating text into various languages using a language model.

🚀 Features
✅ FastAPI-powered REST API
✅ LangChain for prompt management and chaining
✅ Groq model (Gemma2-9b-It) for language tasks
✅ LangServe integration for easy route management
✅ Environment variable-based API key management

⚙️ Environment Setup
Create a .env file in your project directory:

ini
Copy
Edit
GROQ_API_KEY="your_groq_api_key_here"

📂 Project Structure
bash
Copy
Edit
.
├── serve.py       # Main API server
├── .env           # API keys and secrets
└── README.md      # Project documentation

📌 Usage
Run the server
bash
Copy
Edit
python serve.py
By default, the API will be available at:

cpp
Copy
Edit
http://127.0.0.1:8000
You can access the interactive API docs at:

arduino
Copy
Edit
http://127.0.0.1:8000/docs
📤 API Endpoint
POST /chain/invoke
Invoke the translation chain.

Request body example:

json
Copy
Edit
{
  "input": {
    "language": "French",
    "text": "Hello, how are you?"
  }
}
Response example:

json
Copy
Edit
{
  "output": "Bonjour, comment ça va ?"
}
🛠 Code Overview
Prompt template:
The system prompt:

pgsql
Copy
Edit
Translate the following into {language}:
Chain:
ChatPromptTemplate → ChatGroq model → StrOutputParser

LangServe routes:
The chain is exposed at /chain.

💡 Notes
Make sure your Groq API key is active and has enough quota.

You can change the model (e.g., Gemma2-9b-It) by editing serve.py.

Use uvicorn flags if you want auto-reload during development:

bash
Copy
Edit
uvicorn serve:app --reload


=======
🌐 LangChain Translation API
This is a FastAPI server powered by LangChain, LangServe, and Groq that exposes an API for translating text into various languages using a language model.

🚀 Features
✅ FastAPI-powered REST API
✅ LangChain for prompt management and chaining
✅ Groq model (Gemma2-9b-It) for language tasks
✅ LangServe integration for easy route management
✅ Environment variable-based API key management

⚙️ Environment Setup
Create a .env file in your project directory:

ini
Copy
Edit
GROQ_API_KEY="your_groq_api_key_here"

📂 Project Structure
bash
Copy
Edit
.
├── serve.py       # Main API server
├── .env           # API keys and secrets
└── README.md      # Project documentation

📌 Usage
Run the server
bash
Copy
Edit
python serve.py
By default, the API will be available at:

cpp
Copy
Edit
http://127.0.0.1:8000
You can access the interactive API docs at:

arduino
Copy
Edit
http://127.0.0.1:8000/docs
📤 API Endpoint
POST /chain/invoke
Invoke the translation chain.

Request body example:

json
Copy
Edit
{
  "input": {
    "language": "French",
    "text": "Hello, how are you?"
  }
}
Response example:

json
Copy
Edit
{
  "output": "Bonjour, comment ça va ?"
}
🛠 Code Overview
Prompt template:
The system prompt:

pgsql
Copy
Edit
Translate the following into {language}:
Chain:
ChatPromptTemplate → ChatGroq model → StrOutputParser

LangServe routes:
The chain is exposed at /chain.

💡 Notes
Make sure your Groq API key is active and has enough quota.

You can change the model (e.g., Gemma2-9b-It) by editing serve.py.

Use uvicorn flags if you want auto-reload during development:

bash
Copy
Edit
uvicorn serve:app --reload


>>>>>>> 500748a8b9f5dca2d2f758083d35a2da1a4490a9
