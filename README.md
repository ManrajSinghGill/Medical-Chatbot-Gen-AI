# End-to-End Medical Chatbot with Generative AI

This project is a fully functional medical chatbot leveraging Generative AI technologies. It combines the power of GPT, LangChain, and Pinecone for conversational capabilities, search indexing, and retrieval.

## Features
- Conversational AI chatbot
- Medical information retrieval
- End-to-end deployment using Flask

---

### **Step 1: Install Requirements**
Install the required dependencies listed in the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

---

### **Step 2: Configure API Keys**
1. Create a `.env` file in the root directory of the repository.
2. Add the following content to the `.env` file:
```env
PINECONE_API_KEY = "your_pinecone_api_key"
OPENAI_API_KEY = "your_openai_api_key"
```
Replace `your_pinecone_api_key` and `your_openai_api_key` with your actual API keys.

---

### **Step 3: Store Embeddings to Pinecone**
Run the following command to store the embeddings in your Pinecone index:
```bash
python store_index.py
```

---

### **Step 4: Run the Application**
Start the Flask app using the following command:
```bash
python app.py
```

---

### **Step 5: Open the Chatbot**
Open your browser and navigate to:
```
http://localhost:8080
```

---

## **Tech Stack Used**
- **Python**: Core programming language.
- **LangChain**: Used for chaining GPT with search functionalities.
- **Flask**: Web framework for deploying the chatbot.
- **GPT**: Generative AI for conversational capabilities.
- **Pinecone**: Vector database for storing and retrieving embeddings.

---

## **Repository Structure**
```
.
├── app.py                  # Main Flask app
├── store_index.py          # Script to store embeddings into Pinecone
├── requirements.txt        # List of Python dependencies
├── .env                    # API key configuration file
└── README.md               # Project instructions (this file)
```

---

