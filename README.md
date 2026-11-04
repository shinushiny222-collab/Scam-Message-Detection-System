# Scam-Message-Detection-System
## Project Overview

Scam Message Detection System is an AI-powered application that analyzes suspicious messages and identifies possible online scams.

It uses a locally running Large Language Model (LLM) through Ollama to examine messages and generate a safety report.

## Features

- Analyze suspicious SMS, emails and WhatsApp messages.
- Identify possible phishing attempts.
- Detect suspicious payment requests.
- Identify requests for confidential information.
- Classify messages based on risk levels.
- Provide safety recommendations.
- Generate AI-based investigation reports.

## Technologies Used

- Python
- Streamlit
- Ollama
- Gemma 3 (1B)
- Requests
- JSON

## Project Structure

```text
Scam-Message-Detection-System/
│
├── app.py
├── requirements.txt
└── README.md
```

## Installation

### 1. Clone the Repository

```bash
git clone <your-github-repository-url>
```

### 2. Navigate to the Project Folder

```bash
cd Scam-Message-Detection-System
```

### 3. Install Python Dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Install Ollama

Download Ollama from:

https://ollama.com/download

### 5. Download the AI Model

```bash
ollama pull gemma3:1b
```

### 6. Start Ollama

```bash
ollama serve
```

### 7. Run the Application

Open another terminal and execute:

```bash
python -m streamlit run app.py
```

## How It Works

1. The user enters a suspicious message.
2. The application sends the message to the local Ollama API.
3. The Gemma 3 model analyzes the message.
4. The AI identifies possible suspicious indicators.
5. The application generates a detection report.
6. The user receives safety recommendations.

## Risk Classification

- Safe: No obvious suspicious indicators identified.
- Suspicious: Some potential scam indicators detected.
- Dangerous: Multiple serious scam indicators detected.

These classifications are AI-generated assessments and do not independently verify message authenticity.

## Privacy

Messages are sent to the locally running Ollama service for analysis. The application does not require an external AI API key.

## Disclaimer

This application is developed for educational and cybersecurity awareness purposes. AI-generated results may not always be accurate. Always verify suspicious messages through official channels.
