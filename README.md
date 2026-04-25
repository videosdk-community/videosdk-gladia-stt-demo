# VideoSDK x Gladia STT Demo

This example demonstrates how to build a voice assistant using **VideoSDK**'s `Pipeline` with **Gladia**.

![post](https://assets.videosdk.live/images/gladia-post.png)

## Prerequisites

- Python 3.10+
- A [VideoSDK Account](https://dub.sh/BVOvGNr)
- A [Gladia API Key](https://app.gladia.io/apikeys)
- A [Deepgram API Key](https://console.deepgram.com/apikeys)
- A [Google Gemini API Key](https://aistudio.google.com/apikey)

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/videosdk-community/videosdk-gladia-stt-demo.git
    cd videosdk-gladia-stt-demo
    ```

2.  **Create a virtual environment:**

    ```bash
    python -m venv .venv
    ```

    Activate the virtual environment:
    - MacOS/Linux: `source .venv/bin/activate`
    - Windows: `.venv\Scripts\activate`

3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Configuration

1.  **Set up environment variables:**
    Copy the `.env.example` file to `.env`:

    ```bash
    cp .env.example .env
    ```

2.  **Configure API Keys:**
    Open `.env` and fill in your keys:

    ```env
    DEEPGRAM_API_KEY="your_deepgram_api_key"
    GOOGLE_API_KEY="your_google_api_key"
    VIDEOSDK_API_KEY="your_videosdk_api_key"
    VIDEOSDK_SECRET_KEY="your_videosdk_secret_key"
    GLADIA_API_KEY="your_gladia_api_key"
    ```

    **How to get your VideoSDK token:**
    1.  Go to [VideoSDK Dashboard](https://dub.sh/BVOvGNr)
    2.  Navigate to **API Keys** section
    3.  Copy your API Key or generate a new token

    **How to get other API Keys:**
    - **Gemini**: [Google AI Studio](https://aistudio.google.com/apikey)
    - **Deepgram**: [Deepgram Console](https://console.deepgram.com/)
    - **Gladia**: [Gladia Dashboard](https://app.gladia.io/apikeys)

## Usage

Run the agent:

```bash
python main.py
```

## Documentation

- [Gladia STT Plugin Documentation](https://docs.videosdk.live/ai_agents/plugins/stt/gladia)

## VideoSDK Agents

Build and deploy production-ready AI voice & video agents with [VideoSDK](https://videosdk.live). This repo is your central hub for agent templates, feature examples, and everything you need to ship real-world AI-powered applications.

| Resource | Description |
|---|---|
| 🚀 [Use Case Examples](https://github.com/videosdk-live/agents/tree/main/use_case_examples) | Production-ready templates across Customer Support, Healthcare, Tech Support & more |
| ⚡ [Feature Examples](https://github.com/videosdk-live/agents/tree/main/examples) | Always up-to-date examples showcasing the latest VideoSDK Agent features |
| 📖 [AI Agents Docs](https://docs.videosdk.live/ai_agents/introduction) | Full guides, concepts & API references to get you started |

> ⭐ If this helps you, star this repo and [`videosdk-live/agents`](https://github.com/videosdk-live/agents) — it keeps us motivated to ship more!
