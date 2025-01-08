
---

# Local ChatGPT with Llama3.2-Vision

This project provides a local ChatGPT implementation using Llama3.2-Vision. It runs completely offline, allowing you to interact with an AI assistant similar to ChatGPT, powered by the Llama3.2-Vision model.

## Setup Instructions

### Step 1: Clone the Repository
First, clone the repository to your local machine:
```bash
git clone https://github.com/KhuramMurad/local-ChatGPT.git
cd local-ChatGPT
```

### Step 2: Create a Virtual Environment
Create and activate a virtual environment to isolate the project:
```bash
python3 -m venv myenv
source myenv/bin/activate
```

### Step 3: Install Ollama and Dependencies Inside the Virtual Environment
With the virtual environment activated, install Ollama and other dependencies:
```bash
pip install pydantic==2.10.1 chainlit ollama
```

### Step 4: Pull Llama3.2-Vision Model
Download the Llama3.2-Vision model to use with Ollama:
```bash
ollama pull llama3.2-vision
```

### Step 5: Run the Application
Run the Chainlit app:
```bash
chainlit run app.py -w
```

Once the app starts, open it in your browser at:
```plaintext
http://localhost:8000
```

---

## Python Script Overview

The main logic of the project resides in `app.py` and includes:
- **Chat Start**: Initializes the conversation with a greeting message.
- **Tool Step**: Interacts with Llama3.2-Vision and updates the conversation with user input.
- **Main Interaction**: Processes messages and provides AI assistant responses based on Llama3.2-Vision.

## Removing the Setup

To remove the setup:
1. Deactivate and remove the virtual environment:
   ```bash
   deactivate
   rm -rf myenv
   ```
2. Uninstall Python packages:
   ```bash
   pip uninstall pydantic chainlit ollama
   ```

3. Optionally, delete any remaining project files.

---
