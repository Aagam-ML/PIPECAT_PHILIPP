# 🎤 Pipecat AI Voice Assistant

A fully interactive voice assistant powered by a **cascade voice AI pipeline** combining:
**Speech-to-Text (STT) → Large Language Model (LLM) → Text-to-Speech (TTS)**.

Built using **Deepgram**, **OpenAI**, and **Cartesia**, with a web client using **WebRTC** for real-time streaming.

---

## ✨ Features

- 🔊 Real-time smart voice assistant
- 🧠 Works with any OpenAI model
- 🗣️ Choice between **4 high-quality voices**
- 🔗 Web-based interface powered by **SmallWebRTC**
- 🪄 Modular pipeline implementation

---

## 🧱 Tech Stack

| Component | Provider / Framework |
|-----------|---------------------|
| STT (Speech-to-Text) | Deepgram |
| LLM | OpenAI |
| TTS (Text-to-Speech) | Cartesia |
| Transport | SmallWebRTC |
| Server | Python |
| Client | JavaScript / Vite |

---

## 📦 Prerequisites

| Service | Link |
|---------|------|
| OpenAI API | https://platform.openai.com/docs/overview |
| Deepgram API | https://console.deepgram.com/ |
| Cartesia API | https://docs.cartesia.ai/get-started/make-an-api-request |

You will need to obtain API keys for each and configure them in your environment file.

---

## 🚀 Getting Started

### 🖥️ Server Setup

Install my-project with npm

```bash
# Navigate to server directory
cd server
```


```bash
# Install all dependencies
uv sync
```

```bash
# make .env file and paste all apis in it use env.example for an example
.env
```

```bash
# run the server
uv run bot.py
```

### 🌐 Client Setup
Install my-project with npm

```bash
# Navigate to client directory
cd client
```


```bash
# Install all dependencies
npm install
```

```bash
# start development server
npm run dev
```

```bash
# use the application
http://localhost:5173
```

## Project Structure

```
VA/
├── server/              # Python bot server
│   ├── bot.py           # Main bot implementation
│   ├── pyproject.toml   # Python dependencies
│   ├── env.example      # Environment variables template
│   ├── .env             # Your API keys (git-ignored)
│   ├── Dockerfile       # Container image for Pipecat Cloud
│   └── pcc-deploy.toml  # Pipecat Cloud deployment config
├── client/              # Vanilla application
│   ├── src/             # Client source code
│   ├── package.json     # Node dependencies
│   └── ...
├── .gitignore           # Git ignore patterns
└── README.md            # This file
```



