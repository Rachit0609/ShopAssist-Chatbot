ShopAssist 2.0: AI Laptop Recommendation Chatbot
This project is an AI-powered chatbot that recommends laptops based on user needs. It has been upgraded to use Google Gemini's Function Calling feature, allowing the AI to directly call a Python function to search a product database in real-time.

🚀 Key Features
Natural language conversation to understand user requirements.

Uses Function Calling to intelligently search a product database.

Interactive chat loop for a continuous user experience.

⚙️ How to Run
1. Clone the Repository

Bash

git clone https://github.com/YourUsername/ShopAssist-Chatbot.git
cd ShopAssist-Chatbot
(Remember to replace YourUsername with your actual GitHub username.)

2. Install Dependencies
Create a requirements.txt file with the following content:

Plaintext

google-generativeai
pandas
python-dotenv
Then, install the dependencies from your terminal:

Bash

pip install -r requirements.txt
3. Configure API Key
Create a file named .env in the project folder and add your Google Gemini API key to it:

GOOGLE_API_KEY=YOUR_API_KEY_HERE
4. Run the Chatbot
Open the ShopAssist_2.0.ipynb notebook and execute the final cell to start the chat.

Python

run_chatbot()
