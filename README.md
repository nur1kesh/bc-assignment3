# Kazakhstan Constitution QA AI (Powered by Gemini)

This Python application allows users to ask questions about the **Constitution of the Republic of Kazakhstan** using **Google's Gemini AI**. The AI is instructed to answer strictly based on the provided text, ensuring responses are grounded in the actual constitutional document.

---

## 📦 Features

* Loads the Kazakhstan Constitution from a local text file.
* Uses Gemini AI (`gemini-1.5-flash` or configurable model) for question answering.
* Interactive command-line interface.
* Secure handling of API keys using `.env` file or environment variables.

---

## 🚀 Getting Started

### 1. Clone the Repository

git clone https://github.com/yourusername/kazakhstan-constitution-qa.git
cd kazakhstan-constitution-qa

### 2. Install Dependencies

Make sure you have Python 3.7+ installed.

pip install -r requirements.txt

### 3. Add Your Google API Key

Create a .env file in the root directory and add your Google API key:

GOOGLE_API_KEY=your-google-api-key-here

Or set it manually in your terminal session:

export GOOGLE_API_KEY="your-google-api-key-here"

> Note: You must have access to the Google Generative AI API and a valid API key.

### 4. Add the Constitution File

Place the text version of the Kazakhstan Constitution in the project directory and name it g.txt. You can change the filename in the script if needed.

---

## 🧠 Usage

Run the app:

python main.py

You’ll see a prompt where you can ask questions such as:

Your question: What are the fundamental rights of citizens?

To exit, type:

Your question: quit

---

## 🔧 Configuration

Inside the script:

* You can change the Gemini model by editing this line:

model = genai.GenerativeModel('gemini-1.5-flash')

Other options include:

* 'gemini-pro'
* 'gemini-1.5-pro' (better for very large documents)

---

## 📁 File Structure

.
├── main.py                 # Main application script
├── g.txt                   # Constitution text file (you provide this)
├── .env                    # Environment variables (optional)
└── requirements.txt        # Python dependencies

---

## 🛡️ Security Notes

* Avoid hardcoding your API key directly into the code.
* .env file is not included in version control (add it to .gitignore if using Git).
* The AI is instructed to rely only on the text provided, not outside data.

---

## ✅ Requirements

* Python 3.7+
* google-generativeai
* python-dotenv

To install manually:

pip install google-generativeai python-dotenv

---

## 📜 License

This project is open-source and available under the MIT License *(add one if needed)*.

---

## 🙋‍♂️ Questions or Feedback?

Feel free to open an issue or submit a pull request.
