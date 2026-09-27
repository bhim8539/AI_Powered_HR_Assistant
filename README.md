# AI_Powered_HR_Assistant

AI-Powered HR Assistant project demonstrates a Retrieval-Augmented Generation (RAG) pipeline for HR-related queries.

## Project Setup

Follow these steps to set up the project locally:

### 1. Open the project folder
- Navigate to the project directory:
  `AI_Powered_HR_Assistant`
- Make sure the following files are present:
  - `AI_Powered_HR_Assistant.ipynb`
  - `config.json`
  - `Dataset/`

### 2. Create a virtual environment
Open a terminal in the project folder and run:

```bash
python -m venv venv
```

Activate it:

- Windows:
```bash
venv\Scripts\activate
```

- macOS/Linux:
```bash
source venv/bin/activate
```

### 3. Install required Python packages
Install the dependencies needed for the notebook:

```bash
pip install openai langchain langchain-community faiss-cpu pandas numpy jupyter gradio python-dotenv
```

If you are using a different environment or package list, make sure the notebook imports are installed before running it.

### 4. Add your OpenAI API key
Open `config.json` and replace:

```json
{
  "openai": {
    "api_key": "your_api_key_here"
  }
}
```

with your actual OpenAI API key.

### 5. Prepare the dataset
Make sure the files inside the `Dataset/` folder are available and correctly named. The notebook will use this data for retrieval and answer generation.

### 6. Launch Jupyter Notebook
Start the notebook environment:

```bash
jupyter notebook
```

Then open `AI_Powered_HR_Assistant.ipynb` and run the cells in order.

### 7. Run the app
If the project includes a Gradio app or web interface, run the relevant cell or script to launch it in the browser.

### 8. Test the assistant
Ask HR-related questions such as:
- Leave policy
- Employee benefits
- Payroll information
- Workplace guidelines

The system should retrieve relevant context from the dataset and generate a grounded response.

## Notes
- Keep your API key private and do not share it in public repositories.
- If you get import errors, install the missing package using `pip install <package_name>`.
- For production use, use environment variables instead of hardcoding secrets in source files.
