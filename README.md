# 🌍 GlobeNER 2.0 — Offline Multilingual Named Entity Recognition Platform

GlobeNER 2.0 is a full-stack AI-powered Named Entity Recognition (NER) system that extracts structured information from unstructured multilingual text and documents. The system runs fully offline using a locally hosted multilingual NER model and provides interactive analytics and visualization dashboards.

---

## 🚀 Features

- 🔍 Text Analysis — Real-time entity extraction with highlighted results  
- 📂 Batch File Processing — Supports PDF, CSV, JSON, and TXT files  
- 🌎 Multilingual Support — Works with multiple languages including Indian languages  
- 🧠 Offline AI Model — No external API dependency  
- 🧩 Hybrid Extraction — AI model + Regex (Email, Phone, Date, Money)  
- 📊 Analytics Dashboard — Entity distribution and trends  
- 🔗 Knowledge Graph — Visual entity relationship mapping  
- 💾 Persistent Storage — SQLite database  
- ⚡ Fully Offline Processing — Local model inference  

---

## 🏗️ Tech Stack

### Frontend
- React
- Vite
- Tailwind CSS
- Recharts

### Backend
- Node.js
- Express
- TypeScript
- SQLite

### AI Model
- @xenova/transformers
- ONNX Runtime
- Multilingual NER Model

---

## ⚙️ How It Works

Text/File Input → File Parsing → Local AI Entity Extraction → Database Storage → Dashboard Visualization

The system identifies:

- Person names
- Locations
- Organizations
- Email addresses
- Phone numbers
- Dates
- Monetary values

---

## 📦 Installation & Setup

### 1. Clone Repository

```bash
git clone <repository-link>
cd GlobeNER-2.0
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment

Create `.env` file in project root:

```
LOCAL_MODEL_PATH=./local_models
DB_PATH=./globener.db
```

### 4. Download AI Model (One-time setup)

```bash
npm run download:model
```

This downloads the model locally for offline inference.

### 5. Run Application

```bash
npm run dev
```

Open in browser:

```
http://localhost:3000
```

---

## 🧪 Usage

- Paste text for real-time entity extraction
- Upload files (PDF, CSV, JSON, TXT) for batch processing
- View analytics dashboard and knowledge graph visualization

---

## 📁 Project Structure

```
GlobeNER-2.0
│
├── src/                # Frontend components
├── server/             # Backend services
├── local_models/       # Downloaded AI models
├── scripts/            # Model download and testing scripts
├── globener.db         # SQLite database
└── server.ts           # Main server
```

---

## ⚠️ Requirements

- Node.js v20 LTS recommended
- Internet required only for first model download

---

## 🎯 Use Cases

- Document analysis
- Legal text processing
- Financial data extraction
- Customer feedback analysis
- Multilingual text intelligence

---

## 📌 Future Improvements

- Model performance optimization
- Custom entity training
- Enhanced UI/UX
- Scalable deployment
