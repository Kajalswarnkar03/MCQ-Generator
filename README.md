🧠 MCQ Generator Web App
This web application allows users to upload documents (PDF, DOCX, or TXT) and automatically generates multiple-choice questions (MCQs) using Google's Gemini AI model.

🚀 Features
Upload documents in PDF, DOCX, or TXT format.

Specify the number of MCQs to generate.

View MCQs in a user-friendly format.

Download generated questions as TXT and PDF files.

🛠️ Tech Stack
Python (Flask)

HTML/CSS (Jinja2 templates)

Google Generative AI (Gemini)

pdfplumber, docx, FPDF

📁 Project Structure
graphql
Copy
Edit
├── app.py                  # Flask backend application
├── templates/
│   ├── index.html          # Homepage with file upload form
│   └── results.html        # Displays generated MCQs
├── uploads/                # Uploaded user documents (auto-created)
├── results/                # Stores generated TXT and PDF files (auto-created)
└── README.md               # Project documentation
⚙️ Setup Instructions
Clone the repo:

bash
Copy
Edit
git clone https://github.com/yourusername/mcq-generator.git
cd mcq-generator
Install dependencies:

bash
Copy
Edit
pip install flask fpdf pdfplumber python-docx google-generativeai
Set up your Google API Key: Replace the line in app.py with your actual Gemini API key:

python
Copy
Edit
os.environ["GOOGLE_API_KEY"] = "your-google-api-key"
Run the application:

bash
Copy
Edit
python app.py
Open your browser and go to: http://127.0.0.1:5000

📝 Output Format
Each MCQ includes:

A question

Four options (A–D)

Clearly marked correct answer

Example format:

yaml
Copy
Edit
## MCQ
Question: What is the capital of France?
A) Berlin
B) Madrid
C) Paris
D) Rome
Correct Answer: C) Paris
📦 Output Downloads
After generation, users can download:

A plain text file (.txt)

A nicely formatted PDF (.pdf)

💡 Future Improvements
Add support for extracting content from images using OCR

Improve MCQ formatting and validation

User authentication and MCQ history
