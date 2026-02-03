# Heritage Atlas
## Geographical Indication–Based Artisan Commerce Platform

Heritage Atlas is a digital marketplace focused on preserving and promoting India's GI-tagged traditional art forms. The platform organizes artisan products geographically, allowing users to explore crafts based on cultural regions rather than generic product categories.

## Features

- 🗺️ **Map-Centric UI**: Explore crafts by geographical regions
- 🎨 **GI-Tagged Products**: Products organized by Geographical Indications (e.g., Kondapalli, Kalamkari)
- 🔍 **Region-Based Discovery**: Fast filtering using MongoDB aggregation pipelines
- 📸 **Artisan Uploads**: Simple product upload with regional identifiers
- 📖 **Cultural Storytelling**: Rich narratives about traditional art forms
- 🚀 **High Performance**: Optimized queries using MongoDB aggregation

## Tech Stack

- **Frontend**: Modern Web Technologies
- **Backend**: FastAPI
- **Database**: MongoDB (with Aggregation Pipeline)
- **Cloud**: Vercel (Frontend), Render (Backend)

## Project Structure

```
HeritageCraft Atlas/
├── backend/          # FastAPI backend
├── frontend/         # ReactJS frontend
└── README.md
```

## Getting Started

### Prerequisites

- **Python 3.9+**
- **Node.js 18+**
- **MongoDB** (local or [MongoDB Atlas](https://www.mongodb.com/atlas) free tier)

### After cloning on a new device

When you clone this repo on another machine, you **do need to install dependencies** (they are not stored in the repo). Follow the steps below once per device.

### Quick Start

1. **Clone the repository:**
```bash
git clone <repository-url>
cd "HeritageCraft Atlas"
```

2. **Backend Setup** (install Python dependencies and run):
```bash
cd backend
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

pip install -r requirements.txt

# Copy env template and edit if needed
# Windows: copy .env.example .env
# macOS/Linux: cp .env.example .env

uvicorn main:app --reload
```

Backend runs at `http://localhost:8000` · API docs: http://localhost:8000/docs

3. **Seed sample data (optional):**
```bash
cd backend
python seed_data.py
```

4. **Frontend Setup** (install Node dependencies and run):
```bash
cd frontend
npm install

# Create .env with: REACT_APP_API_URL=http://localhost:8000

npm start
```

Frontend runs at `http://localhost:3000`

## Environment Variables

### Backend (.env)
```
MONGODB_URI=mongodb://localhost:27017/heritagecraft
DATABASE_NAME=heritagecraft
CORS_ORIGINS=http://localhost:3000
```

### Frontend (.env)
```
REACT_APP_API_URL=http://localhost:8000
```

## Deployment

- **Frontend**: Deploy to Vercel
- **Backend**: Deploy to Render

## Objectives

- ✅ Digitally preserve GI-tagged arts
- ✅ Enable region-based product discovery
- ✅ Support artisan-first commerce
- ✅ Use aggregation for high-performance filtering
- ✅ Promote cultural storytelling
- ✅ Enable future e-commerce integrations
- ✅ Encourage fair visibility for rural artists
