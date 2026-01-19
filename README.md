# VideoSDK + Gladia STT Demo

This example demonstrates how to build a voice assistant using **VideoSDK**'s `CascadingPipeline` with **Gladia**.

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
    VIDEOSDK_AUTH_TOKEN="your_videosdk_auth_token"
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

The agent will join the room (as configured in `main.py`) and wait for you to speak.

## Documentation

- [Gladia STT Plugin Documentation](https://docs.videosdk.live/ai_agents/plugins/stt/gladia)
