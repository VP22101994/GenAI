# 🚀 How to Run the App

Follow these steps to set up and run the application:

---

## 1️⃣ Create an Account in LangChain  
- Visit the [LangChain website](https://www.langchain.com/) (or your designated platform URL).  
- Sign up for a new account or log in if you already have one.

---

## 2️⃣ Generate a LangChain API Key  
- After logging in, go to **Account Settings** → **API Keys** (or similar).  
- Create a new API key.  
- **Copy and store the API key securely** — you’ll need it for the app.

---

## 3️⃣ Configure the App with Your LangChain API Key  
- Open the project folder.
- Locate the configuration file (e.g., `.env`, `config.py`) or create a `.env` file if it doesn't exist.  
- Add your LangChain API key:


- Alternatively, set it as an environment variable:
- **Linux / macOS**
  ```bash
  export LANGCHAIN_API_KEY=your_api_key_here
  ```
- **Windows (CMD)**
  ```cmd
  set LANGCHAIN_API_KEY=your_api_key_here
  ```
- **Windows (PowerShell)**
  ```powershell
  $env:LANGCHAIN_API_KEY="your_api_key_here"
  ```

---

## 4️⃣ Install Dependencies  
- Open your terminal or command prompt in the project folder.

- Run:
```bash
pip install -r requirements.txt


streamlit run your_app.py


Notes

Ensure you are using Python 3.8+.

Make sure your API key has the required permissions for the app’s functionality.

If you run into issues, check that all dependencies were installed correctly and your API key is valid.


Monitor Your App in LangSmith
You can monitor your app’s responses, model usage, and performance directly in LangSmith — LangChain’s observability platform.

Visit LangSmith and log in with your LangChain account.

Use this to track traces, debug chains, and optimize your app.