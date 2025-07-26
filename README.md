🤖 Chat-Bot-AI
A simple Flask web application that uses Cohere API to create an AI-powered chatbot.

✨ Features
✔️ Flask-based backend
✔️ AI responses using Cohere Command R
✔️ Simple HTML interface

📂 Project Structure
bash
Copy code
📁 Chat-Bot-AI
 ├── 📄 app.py           # Main Flask app
 ├── 📄 .env             # API Key (Cohere)
 ├── 📄 requirements.txt # Dependencies
 └── 📁 templates/
      ├── index.html     # Home page
      └── chatbot.html   # Chat UI
🚀 How to Run
✅ 1. Clone the Repository
bash
Copy code
git clone https://github.com/Rahitya86/Chat-Bot-AI.git
cd Chat-Bot-AI
✅ 2. Install Dependencies
bash
Copy code
pip install flask cohere python-dotenv
✅ 3. Add Your API Key
Create a .env file in the project folder:

ini
Copy code
COHERE_API_KEY=your_api_key_here
✅ 4. Run the App
bash
Copy code
python app.py
Open in your browser: http://127.0.0.1:5000/

🌐 Pages
🏠 index.html → Home page

💬 chatbot.html → Chat interface

⚙️ Tech Used
🐍 Python (Flask)

🌐 HTML, CSS, JS

🤖 Cohere API
