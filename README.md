
ShopAssist 2.0: An AI Laptop Recommendation Chatbot
This project is an advanced version of a conversational AI agent designed to recommend laptops. It's an enhancement of an original proof-of-concept, refactored to use the powerful Function Calling feature of Google's Gemini API.

🚀 Project Overview
The original ShopAssist chatbot relied on complex prompt engineering to have a conversation and guess the user's needs. It would then try to format its understanding as a string, which the Python code would have to parse. This process was brittle and prone to errors.

ShopAssist 2.0 re-architects the system into a modern, tool-augmented agent. The AI's role is elevated from a simple text generator to an intelligent orchestrator that can use Python functions as "tools" to perform real-world actions.

When a user asks for a laptop, the AI now has a natural conversation to gather the requirements and then makes a direct, structured call to a Python function (find_laptops) to search the product database.

Key Features
Natural Language Understanding: Engages in a multi-turn conversation to understand a user's needs.

Intelligent Tool Use: Utilizes Function Calling to execute a local Python function to search and score laptops.

Dynamic Recommendations: Filters products by budget and scores them against user preferences like portability, GPU power, and display quality.

Interactive Chat Loop: Provides a continuous, conversational experience until the user decides to exit.

Secure API Key Management: Uses a .env file to keep secret keys out of the source code.

🛠️ Technologies Used
Python 3.9+

Google Gemini API (google-generativeai) for the core LLM.

Pandas for data manipulation and searching the laptop database.

Jupyter Notebook for development and demonstration.

python-dotenv for managing environment variables securely.

⚙️ Setup and Installation
Follow these steps to run the project on your local machine.

1. Clone the Repository
First, clone this repository to your local machine.

Bash

git clone https://github.com/YourUsername/ShopAssist-Chatbot.git
cd ShopAssist-Chatbot
(Remember to replace YourUsername with your actual GitHub username.)

2. Install Dependencies
This project uses a few Python libraries. It's recommended to create a requirements.txt file for easy installation.

Create a requirements.txt file with the following content:

google-generativeai
pandas
python-dotenv
Then, install the dependencies:

pip install -r requirements.txt

3. Configure Your API Key
The application loads your Google Gemini API key from an environment file for security.

Create a file named .env in the root directory of the project.

Open the .env file and add the following line, replacing YOUR_API_KEY_HERE with your actual key from Google AI Studio:

GOOGLE_API_KEY=YOUR_API_KEY_HERE

▶️ How to Run
Once the setup is complete, you can run the chatbot.

Open the ShopAssist_2.0.ipynb file in Jupyter Notebook.

Run the cells in order from top to bottom.

The final cell will call the run_chatbot() function and start the interactive chat in your notebook.


# The final step is to call this function to start the chat
run_chatbot()
