Chat-Bot-AI
A simple Flask-based chatbot web application that uses Cohere's Command R model for AI-powered responses.

Features
✅ Flask backend for handling chat requests
✅ Two web pages:

index.html – Landing page

chatbot.html – Chat interface
✅ Integration with Cohere API
✅ Environment variable support using .env

Project Structure
bash
Copy code
Chat-Bot-AI/
│
├── templates/
│   ├── index.html        # Home page
│   ├── chatbot.html      # Chat interface page
│
├── app.py                # Flask application
├── .env                  # Environment variables (COHERE_API_KEY)
├── requirements.txt      # Dependencies
└── README.md
Installation & Setup
1. Clone the Repository
bash
Copy code
git clone https://github.com/Rahitya86/Chat-Bot-AI.git
cd Chat-Bot-AI
2. Create a Virtual Environment
bash
Copy code
python -m venv venv
source venv/bin/activate     # Mac/Linux
venv\Scripts\activate        # Windows
3. Install Dependencies
bash
Copy code
pip install flask cohere python-dotenv
4. Configure Environment Variables
Create a file named .env in the root directory:

ini
Copy code
COHERE_API_KEY=your_cohere_api_key_here
5. Run the Application
bash
Copy code
python app.py
Access the app at:
http://127.0.0.1:5000/

How It Works
index.html → Displays a welcome page with a link to the chatbot.

chatbot.html → Provides a text input for users to chat with the AI.

POST /chat API → Accepts JSON:

json
Copy code
{ "message": "Hello" }
Returns:

json
Copy code
{ "response": "Hi! How can I help you?" }
Example API Call
bash
Copy code
curl -X POST http://127.0.0.1:5000/chat \
-H "Content-Type: application/json" \
-d '{"message":"Hello"}'
Dependencies
Flask

Cohere

python-dotenv

Install them with:

bash
Copy code
pip install -r requirements.txt
