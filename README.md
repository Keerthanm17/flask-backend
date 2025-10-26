# 🎤 gTTS Flask Backend Microservice

A lightweight and robust Flask-based microservice for **Text-to-Speech (TTS)** generation using the popular `gTTS` library (Google Text-to-Speech). This backend is designed to handle multilingual audio generation, supporting a variety of Indian languages, and can be easily integrated into larger projects for text-to-audio conversion.

## ✨ Features

* **Multilingual Support:** Supports several languages including Hindi (`hi`), Kannada (`kn`), Telugu (`te`), Tamil (`ta`), Marathi (`mr`), Gujarati (`gu`), Bengali (`bn`), Punjabi (`pa`), Odia (`or`), and English (`en`).
* **Simple REST API:** Provides a clean `/tts` endpoint for generating audio files.
* **CORS Enabled:** Configured with `Flask-CORS` to allow requests from any frontend application.
* **Health Check:** Includes a `/health` endpoint for monitoring service status.
* **Language Listing:** A `/languages` endpoint to easily retrieve all supported language codes.
* **Ephemeral Storage:** Generates and serves MP3 files from a temporary directory, ensuring a clean and stateless service.

## 🚀 Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You need **Python 3.x** and **`pip`** installed on your system.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
    cd YOUR_REPO_NAME
    ```

2.  **Install dependencies:**
    The `setup.py` script simplifies the installation process by creating a `requirements.txt` file and installing all necessary packages.

    ```bash
    python setup.py
    ```
    *Alternatively, you can install them manually:*
    ```bash
    pip install -r requirements.txt
    ```
    The required packages are:
    * [cite_start]`Flask==2.3.3` [cite: 1]
    * [cite_start]`Flask-CORS==4.0.0` [cite: 1]
    * [cite_start]`gTTS==2.4.0` [cite: 1]
    * [cite_start]`Werkzeug==2.3.7` [cite: 1]

## ⚙️ Running the Server

Start the Flask application using the following command:

```bash
python app.py
