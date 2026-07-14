# Code Assistant Application — Powered by CodeLlama (Llama2)

## Project Overview
This project is a **production-grade AI Coding Assistant**, engineered using [**Meta’s CodeLlama**](https://ollama.com/library/codellama), [**LangChain**](https://www.langchain.com/), and [**Gradio**](https://www.gradio.app/). It delivers an intelligent, context-aware coding experience that mimics real-time pair programming. The assistant not only generates accurate code but also maintains conversational memory to deliver consistent, relevant guidance across interactions.

<br>

## Key Technologies & Architecture
-   **CodeLlama via Ollama** : Utilized for state-of-the-art code generation and natural language understanding. It powers the assistant’s ability to provide real-time, intelligent coding suggestions tailored to the user’s query.
-   **LangChain** : Enables dynamic prompt management and **contextual memory**, ensuring that the assistant maintains coherence across multi-turn conversations.
-   **Gradio** : Offers a minimal yet powerful web-based interface that allows developers to interact seamlessly with the assistant—send prompts, receive responses, and view conversation history—all in real time.

<br>

## How to Run the Project ?
(NOTE : This project was carried out on a [Macintosh](https://www.apple.com/mac/) machine)
### **1. Clone the Repository**
Clone the repository to your local machine :
```bash
git clone https://github.com/SoubhikSinha/Code-Assistant-Application-CodeLlama-Llama2.git

```

<br>

### **2. Create a Virtual Environment**
Navigate to the repository's root directory and create a Conda virtual environment :
```bash
conda create -p ./venv python=3.11 -y
```

<br>

### **3. Activate the Conda Environment**
Activate the newly created environment :
```bash
conda activate venv/
```

<br>

### **4. Install Required Libraries**
Install all the necessary dependencies :
```bash
pip install -r requirements.txt
```

<br>

### **5. Install Ollama**
Ollama is required to run the CodeLlama model. Follow the official installation guide for your operating system:
-   Install Ollama : https://ollama.com/download
<br>

After successful installation, verify the installation by running :
```bash
ollama --version
```

<br>

### **6. Run CodeLlama Model**
Once Ollama is installed, run the following command to execute CodeLlama :
```bash
ollama run CodeLlama
```

<br>

### **7. Create a Custom Model (CodeGuru)**
Generate a new custom model named "codeguru" using the `modelfile`:
```bash
ollama create codeguru -f modelfile
```

<br>

### **8. Run the CodeGuru Model**
Execute the following command to run the newly created `codeguru` model :
```bash
ollama run codeguru
```

<br>

### **9. Launch the Gradio Interface**
Finally, start the Python application to launch the Gradio-based interface :
```bash
python app.py
```
Once executed, the application will be available for interaction via a web-based interface.
