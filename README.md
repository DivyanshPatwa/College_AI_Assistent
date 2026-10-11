# 🎓 College AI Assistant

An AI-powered College Assistant built with Python and Flask that helps students with calculations, attendance management, timetable analytics, and document-based question answering.

## ✨ Features

- 🤖 **AI Chat Assistant:** Answers general questions using Google Gemini.
- 🧮 **Calculator:** Solves mathematical expressions.
- 📅 **Timetable Analytics:** Displays scheduled classes and subject-wise lecture counts.
- 📝 **Attendance Management:** Marks attendance and checks attendance percentages and records.
- 📄 **Document Reader:** Supports PDF, DOCX, and TXT files.
- 💬 **Document Q&A:** Answers questions based on uploaded documents.
- 🛠️ **Tool Tracking:** Displays which tool was used to generate a response.

## 🛠️ Technologies Used

- Python
- Flask
- Google Gemini API
- Hugging Face Inference API (provider code included; API access requires available credits)
- SQLite
- HTML, JavaScript
- PyMuPDF
- python-docx

## 📁 Project Structure

```text
College-AI-Assistant/
├── app.py
├── document_reader.py
├── requirements.txt
├── .gitignore
├── templates/
│   └── index.html
├── tools/
│   ├── attendance.py
│   ├── calculator.py
│   └── timetable.py
├── providers/
│   └── huggingface_provider.py
└── test_*.py
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd College-AI-Assistant
```

Replace `YOUR_REPOSITORY_URL` with your GitHub repository URL.

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Configure environment variables

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your_gemini_api_key
HF_TOKEN=your_hugging_face_token
```

Use your own API keys. Never upload your `.env` file to GitHub.

### 5. Run the application

```bash
python app.py
```

Open the following address in your browser:

```text
http://127.0.0.1:5000
```

## 🧪 Testing

Run the available test scripts individually:

```bash
python test_final.py
python test_final_attendance.py
python test_document_reader.py
python test_upload.py
python test_huggingface.py
```

Some tests may require valid API access or a working local environment.

## 🔐 Security

- API keys are stored in environment variables.
- The `.env` file is excluded through `.gitignore`.
- The virtual environment and local database files are excluded from version control.
- Uploaded documents are excluded from Git tracking by default.

## 🚀 Future Improvements

- Integrate additional LLM providers.
- Improve automatic tool selection.
- Add a student-friendly interface.
- Deploy the application to a hosting platform.
- Add authentication and personalized student profiles.

## 👨‍💻 About

This project demonstrates the use of Python, Flask, AI APIs, document processing, and modular tools to build a useful college assistant.

**Project:** College AI Assistant  
**Status:** In Development
