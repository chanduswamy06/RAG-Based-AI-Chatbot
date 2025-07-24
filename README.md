🤖 RAG-Based AI Chatbot – Built by Chandu

A simple, local app to help you chat with your PDFs. Upload documents, turn them into searchable embeddings, and ask questions using a smart chatbot—all powered by open-source tools and running on your machine via Docker.


✅ What You Can Do with This App

Upload PDFs and view them directly in the app
Generate embeddings for those documents, making them searchable
Chat with your documents using an AI assistant that actually understands the content
Nice interface with emojis, responsive layout, and clean navigation
Get in touch or contribute via GitHub if you'd like to collaborate

🧰 Tech Behind the Scenes

Everything runs locally, using open-source tools:
LangChain – manages the workflow: embedding, storage, chat logic
Unstructured – handles PDF processing and text extraction
BGE Embeddings (from HuggingFace) – creates vector representations of your docs
Qdrant – fast local vector database, running in a Docker container
LLaMA 3.2 via Ollama – serves as the local language model for smart replies
Streamlit – powers the web UI so you can interact with everything easily

📁 Folder Overview

Here’s a quick look at the project structure:
document_buddy_app/
│── logo.png          # App logo
├── new.py            # Main Streamlit app file
├── vectors.py        # Embedding logic
├── chatbot.py        # Chat interaction logic
├── requirements.txt  # Python dependencies

🏃 How to Set It Up (Locally)

Step 1: Clone the Repository
git clone https://github.com/chanduswamy06/RAG-Based-LLM-Chatbot.git
cd RAG-Based-LLM-Chatbot
Step 2: Create a Python Environment
Pick one of the two options:
Option A: Use venv
Windows
python -m venv venv
venv\Scripts\activate
macOS/Linux
python3 -m venv venv
source venv/bin/activate
Option B: Use Anaconda
conda create --name chatbot python=3.10
conda activate chatbot
Step 3: Install the Dependencies
pip install -r requirements.txt
Step 4: Launch the App
streamlit run new.py
If your browser doesn’t open automatically, go to the link in your terminal (usually http://localhost:8501).