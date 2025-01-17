# Briefly-AI

<img src="https://github.com/deepparekh02/ai-assistant/assets/65657471/00888051-d86e-4562-9eb2-dfc90bf3402c" width=400>

## Table of Contents
- [Description](#description)
- [Inspiration](#inspiration)
- [Screenshots](#screenshots)
- [Technologies and Libraries](#technologies-and-libraries)
- [Main Features](#main-features)
- [Possible Upgrades](#possible-upgrades)
- [How to Use](#how-to-use)
- [Installation](#installation)

## Description

Briefly AI is a cutting-edge AI Assistant designed to streamline your communication management. Leveraging advanced AI models and APIs, Briefly AI generates concise summaries for emails and Slack messages, drafts intelligent email responses, and automates these tasks for continuous operation and convenience.

## Inspiration

The inspiration for this AI Assistant came from my own struggle to keep up with the loads of emails and Slack messages I receive daily. As an undergraduate juggling classes, projects, and internships, I found myself spending way too much time trying to sift through endless threads of messages and emails. I thought, "There has to be a smarter way to handle this!"

That's when I decided to harness the power of AI to help me out. I wanted something that could give me quick summaries and draft responses so I could focus on more important things—like coding, studying, or, let's be honest, binge-watching my favorite shows. This project was born out of a need for more efficiency and a desire to see how far I could push AI to make my life easier. By the way, if you have read this far, let me tell you that this readme file was written by an LLM too.

## Screenshots

<img width="500" alt="demo-1" src="https://github.com/deepparekh02/briefly-ai/assets/65657471/1867060e-71d5-4bb6-9c44-a93aa20b4869">
<img width="500" alt="demo-2" src="https://github.com/deepparekh02/briefly-ai/assets/65657471/e18aa0e3-1631-4ac2-9e11-b091340133f5">


## Technologies and Libraries

- **Frontend Technologies:**
  - `Angular` for a sleek and responsive user interface
  - `Ngx-Markdown` for rendering Markdown content
- **Backend Technologies:**
  - `Python` for robust backend operations
  - `Flask` for a lightweight and efficient web framework
- **Google Cloud APIs for seamless integration and authentication:**
  - `google-auth`
  - `google-auth-oauthlib`
  - `google-auth-httplib2`
  - `google-api-python-client`
- **Environment Management:**
  - `python-dotenv` for secure credential management
- **AI and Machine Learning:**
  - `google-generativeai` for state-of-the-art language models
- **Communication Platform Integration:**
  - `slack-sdk` for Slack integration
- **Containerization and Orchestration:**
  - `Docker` for containerizing the application
  - `Kubernetes` for deploying and managing containers
  - `Nginx` for serving the frontend and proxying API requests
- **Others:**
  - `requests` for handling HTTP requests
  - `flask-cors` for handling cross-origin requests

## Main Features

- **Advanced Email Summarization:** Utilizes Gemini AI to generate insightful and concise summaries of email threads using sophisticated prompt engineering techniques.
- **Intelligent Slack Summarization:** Produces comprehensive summaries of Slack conversations, ensuring users stay updated without reading every message.
- **AI-Driven Email Response Drafting:** Employs machine learning algorithms to draft contextually relevant email responses, tailored to user preferences and communication style.
- **Automated and Secure Workflow:** Periodically performs tasks using credentials securely stored in a `.env` file, ensuring data privacy and continuous operation.
- **Seamless AI API Integration:** Integrates with Google Generative AI APIs to harness the full potential of LLMs for natural language understanding and generation.
- **User-Friendly Interface:** A modern and sleek frontend built with Angular, providing an intuitive user experience.
- **Multi-Platform Support:** Supports both email and Slack integrations, with future plans for additional platforms.
- **Real-Time Updates:** Keeps you informed with real-time summaries and drafts, enhancing productivity and efficiency.

## Possible Upgrades

- Add Discord Support.
- Add Whatsapp Business Support.
- Add Microsoft Teams Support.

## How to Use

1. **Enter your credentials:** Input your Google and Slack credentials securely into form.
2. **Specify the time range:** Define the number of hours for which you want to generate summaries.
3. **Generate Summaries:** Click on the respective buttons to generate email or Slack summaries.
4. **Draft Responses:** Use the AI-driven drafting feature to automatically generate email responses.

## Installation

### Prerequisites
- Python 3.x
- Node.js and npm (for the Angular frontend)
- Docker and Docker Compose
- Minikube (for Kubernetes)
- kubectl (Kubernetes command-line tool)
- Helm (Kubernetes package manager)

### Backend Setup
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/briefly-ai.git
    cd briefly-ai/backend
    ```
2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```
    
5. Run the backend server:
    ```bash
    python app.py
    ```

### Frontend Setup
1. Navigate to the frontend directory:
    ```bash
    cd ../frontend
    ```
2. Install the required packages:
    ```bash
    npm install
    ```
3. Run the Angular development server:
    ```bash
    ng serve
    ```

### Docker Setup

1. Build and run the Docker containers using Docker Compose:
    ```bash
    docker-compose up --build
    ```

### Kubernetes Setup

1. Start Minikube:
    ```bash
    minikube start
    ```

2. Enable Ingress in Minikube:
    ```bash
    minikube addons enable ingress
    ```

3. Deploy the application using Helm:
    ```bash
    cd ../k8s
    helm install briefly-ai .
    ```

### Accessing the Application
1. Use the following command to get the URL for accessing the frontend:
    ```bash
    minikube service briefly-ai-frontend
    ```
2. Open your web browser and navigate to the provided URL to access Briefly AI.
