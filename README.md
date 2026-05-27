# Real-time AI GYM Coach

Your form. Analyzed. Corrected. In milliseconds.
An AI-powered, real-time gym trainer that watches every rep and provides instant, actionable feedback to perfect your form and count your reps, all without any extra hardware — just your webcam!

[![Live Demo](https://img.shields.io/badge/Live_Demo-Try_it_live-blue)](https://realtime-ai-gymcoach.netlify.app/)

## 🚀 Features

- **Pose Detection**: Advanced computer vision to track your body mechanics in real-time.
- **Audio Feedback**: Instant voice coaching tells you exactly what to fix during your workout.
- **Rep Counter**: Accurately counts your reps and tracks sets and duration.
- **Works in Real-time**: Ultra-low latency analysis directly in your browser.
- **Dashboard & History**: Tracks your past exercises and stores session details securely in a local database.

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3 (Vanilla, custom UI/UX)
- **Backend / Web App**: Python, [Streamlit](https://streamlit.io/)
- **Computer Vision**: [MediaPipe](https://developers.google.com/mediapipe) for pose estimation, OpenCV
- **Real-time Video Streaming**: `streamlit-webrtc`
- **AI & Coaching**: Groq API for intelligent feedback, `gTTS` for text-to-speech audio coaching
- **Database**: SQLite (built-in)

## 📁 Project Structure

- `Frontend/`: Contains the static HTML/CSS files for the beautiful, responsive landing page.
- `Backend/`: Contains the Streamlit web application, including the core computer vision and AI coaching services.

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.8+
- Git

### 1. Clone the repository
```bash
git clone https://github.com/RushdaBaqui-08/AI-Real-Time-GYM-Coach.git
cd AI-Real-Time-GYM-Coach
```

### 2. Setup the Backend (Streamlit App)
Navigate to the backend directory and set up a virtual environment:
```bash
cd Backend
python -m venv myenv
source myenv/bin/activate  # On Windows use: myenv\Scripts\activate
```

Install the dependencies:
```bash
pip install -r requirements.txt
```

### 3. Environment Variables
Create a `.env` file in the `Backend/` directory and add your Groq API Key (required for AI voice coaching feedback):
```ini
GROQ_API_KEY=your_groq_api_key_here
```

### 4. Run the Application
Run the Streamlit app locally:
```bash
streamlit run main.py
```
The application will be accessible at `http://localhost:8501` (or whichever port Streamlit assigns).

### 5. View the Frontend
To view the custom landing page, simply open `Frontend/index.html` in your browser, or start a local python server:
```bash
cd ../Frontend
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000`.

## 🤝 Let's Connect
Built by a human. Backed by data. Open to opportunities in ML engineering, computer vision, and AI product roles.

- **LinkedIn**: [Rushda Baqui](https://www.linkedin.com/in/rushda-baqui-945581276/)
- **GitHub**: [@RushdaBaqui-08](https://github.com/RushdaBaqui-08)
- **Email**: [rushdabaqui@gmail.com](mailto:rushdabaqui@gmail.com)
