# 🤖 Generative AI Video Summarizer


A Generative AI-based web application that takes a **YouTube video URL**, retrieves its available transcript/captions, and generates a concise summary using a pretrained **BART** model.

## 📸 Application Screenshot

![Generative AI Video Summarizer](video summarizer.png)

The application is built using **Python** and **Gradio**.


---


## ✨ Features


- Accepts YouTube video URLs
- Extracts the YouTube video ID
- Retrieves the available transcript/captions
- Splits long transcripts into smaller chunks
- Summarizes the transcript using `facebook/bart-large-cnn`
- Displays the final summary in a simple Gradio web interface
- Uses GPU automatically when CUDA is available
- Shows readable error messages when processing fails


---


## 🛠️ Technologies Used


- **Python**
- **Gradio** – Web interface
- **YouTube Transcript API** – Transcript retrieval
- **Hugging Face Transformers** – NLP summarization
- **BART (`facebook/bart-large-cnn`)** – Pretrained summarization model
- **PyTorch** – Model execution


---


## 📂 Project Structure


```text
generative-ai-video-summarizer/
│
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
⚙️ Installation
1. Clone the repository
git clone https://github.com/YOUR-USERNAME/generative-ai-video-summarizer.git
cd generative-ai-video-summarizer
2. Create a virtual environment
Windows
python -m venv venv
venv\Scripts\activate
macOS/Linux
python3 -m venv venv
source venv/bin/activate
3. Install dependencies
pip install -r requirements.txt
▶️ Run the Application

Run:

python app.py

Gradio will provide a local URL in the terminal.

Open that URL in your browser.

🧠 How It Works
YouTube URL
     ↓
Extract Video ID
     ↓
Retrieve YouTube Transcript
     ↓
Split Transcript into Chunks
     ↓
BART Summarization
     ↓
Final Summary
     ↓
Gradio Web Interface
📌 Example

Enter a YouTube URL such as:

https://www.youtube.com/watch?v=VIDEO_ID

Then click:

Summarize Video

The application retrieves the available transcript and generates a concise summary.

⚠️ Limitations
The video needs to have an accessible transcript/captions.
Videos without an available transcript may return an error.
BART is a pretrained summarization model and may occasionally omit details or produce imperfect summaries.
The first run may take time because the BART model must be downloaded.
Long videos may take longer to summarize.
🚀 Future Improvements
Add automatic language selection
Support additional summarization models
Generate bullet-point key takeaways
Add transcript download
Add summary export as PDF/TXT
Add video title and duration information
Improve support for videos without captions
👩‍💻 Project
Generative AI Video Summarizer

Built as a Generative AI / NLP project using:

Python
Hugging Face Transformers
BART
YouTube Transcript API
Gradio
PyTorch
