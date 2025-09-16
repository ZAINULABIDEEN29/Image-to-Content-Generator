[No content]
# ImagePrompt: AI-Powered Image to Prompt Generator

Transform your images into detailed prompts and tags using advanced AI technology. Perfect for artists, content creators, and AI enthusiasts.

## 🚀 Overview
ImagePrompt is a full-stack web application that uses state-of-the-art BLIP AI models to analyze images and generate:
- **Danbooru-style tags** for categorization and AI art generation
- **Descriptive prompts** for use in Stable Diffusion, Midjourney, DALL-E, and more
- **Confidence scores** to indicate analysis reliability
- **NSFW support** with age verification

## 🖼️ Features
- **BLIP AI Powered:** Accurate image understanding and caption generation
- **Danbooru/Gelbooru Tags:** Perfect for anime, digital art, and content organization
- **NSFW Analysis:** Age-confirmed, uncensored tag generation for mature content
- **Lightning Fast:** Optimized models for quick results
- **Secure & Private:** Images processed securely, never stored permanently
- **Modern UI:** Beautiful React + Tailwind CSS frontend

## 🏗️ Project Structure

```
Project-ai/
├── client/   # React frontend (Vite, Tailwind)
│   ├── src/
│   │   ├── components/   # UI components (Navbar, Hero, UploadCard, etc.)
│   │   ├── services/     # API service (api.js)
│   │   └── ...
│   ├── public/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── server/   # FastAPI backend (Python)
│   ├── main.py           # API entrypoint
│   ├── requirements.txt  # Python dependencies
│   ├── models/           # Pydantic response models
│   ├── services/         # BLIP image analyzer
│   └── utils/            # File validation utilities
└── Readme.md
```

## ⚡️ Quick Start

### 1. Clone the repo
```sh
git clone https://github.com/ZAINULABIDEEN29/Image-to-Content-Generator.git
cd Project-ai
```

### 2. Start the Backend (FastAPI)
```sh
cd server
python -m venv venv
venv\Scripts\activate  # On Windows
pip install -r requirements.txt
python main.py
# API runs at http://localhost:8000
```

### 3. Start the Frontend (React)
```sh
cd client
npm install
npm run dev
# App runs at http://localhost:5173
```

## 🛠️ Usage
1. Open the app in your browser
2. Upload an image (JPG, PNG, WebP, max 10MB)
3. Choose SFW or NSFW mode (NSFW requires age confirmation)
4. Get tags, prompt, and confidence score instantly
5. Use results for AI art, content creation, or organization

## 🧩 API Endpoints
- `POST /api/validate-upload` — Validate image file
- `POST /api/analyze` — Analyze image (SFW/NSFW)
- `POST /api/analyze-sfw` — SFW analysis
- `POST /api/analyze-nsfw` — NSFW analysis (age confirmed)
- `GET /api/info` — API info
- `GET /health` — Health check

## 📦 Tech Stack
- **Frontend:** React, Vite, Tailwind CSS
- **Backend:** FastAPI, BLIP (transformers), Torch, Pillow

## 📝 License & Legal
- By using this service, you confirm you are 18+ and agree to our terms
- No illegal content allowed
- Images are processed securely and not stored

---

Made with ❤️ for the AI community by [ZAINULABIDEEN29](https://github.com/ZAINULABIDEEN29)
