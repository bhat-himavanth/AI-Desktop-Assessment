#  AI-Powered Desktop Assistant

A real-time multimodal desktop assistant built with **Python, Computer Vision, Speech Recognition, and Desktop Automation**.

The project enables hands-free interaction with a computer using **voice commands, hand gestures, and eye movements**.

##  Features

*  Voice-controlled desktop automation
*  AI-based hand landmark detection
*  Gesture-controlled virtual mouse
*  Eye-controlled cursor and blink-based clicking
*  Hand gesture-based volume control
*  Google, YouTube, Wikipedia, Weather and News integration
*  Email automation
*  Text-to-speech responses
*  Multithreaded real-time processing

##  How It Works

```text
User Input
   │
   ├── Voice ──→ Speech Recognition ──→ Command Processing
   │                                      │
   ├── Hand ──→ MediaPipe Landmarks ──────┤
   │                                      │
   └── Eye ───→ Face Mesh Landmarks ──────┘
                                          │
                                          ▼
                                   Action Execution
                                          │
                         ┌────────────────┼────────────────┐
                         ▼                ▼                ▼
                     Desktop           Mouse           External
                     Control           Control          Services
```

The project uses **pre-trained AI/ML models for perception** and combines their outputs with rule-based decision logic to perform system actions.

##  Tech Stack

* **Python**
* **OpenCV** – image/video processing
* **MediaPipe** – hand and facial landmark detection
* **SpeechRecognition** – speech-to-text
* **pyttsx3** – text-to-speech
* **PyAutoGUI** – mouse/system automation
* **Requests** – API integration
* **PyWhatKit** – web automation
* **SMTP** – email automation
* **Threading** – concurrent execution

##  Project Structure

```text
AI-Desktop-Assistant/
│
├── main.py              # Main assistant and command controller
├── online.py            # API and online service functions
├── virtualmouse.py      # Hand gesture virtual mouse
├── volumetest.py        # Gesture-based volume control
├── fastmouse.py         # Eye-controlled mouse
├── head.py              # Facial/eye tracking
├── conv.py              # Assistant responses
│
├── requirements.txt
├── .env.example
├── .gitignore
└── README.md
```

##  Installation

```bash
git clone https://github.com/<your-username>/AI-Desktop-Assistant.git
cd AI-Desktop-Assistant

python -m venv venv
venv\Scripts\activate

pip install -r requirements.txt
```

Configure the required API credentials in `.env` and run:

```bash
python main.py
```

##  Security

API keys, email credentials, and other secrets must **not** be committed to the repository.

Use environment variables through `.env` and keep the file excluded using `.gitignore`.

##  Future Improvements

* LLM-based natural-language command understanding
* Multimodal AI agent architecture
* Contextual conversation memory
* Custom gesture classification model
* Offline speech recognition
* Face/voice authentication
* Cross-platform support

