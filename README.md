# 🌍 Global Disaster Alert System

A real-time, production-ready platform that provides live updates about natural disasters happening across the globe. Designed to help people stay informed and safe, this system fetches verified disaster data from trusted sources and displays it in a clean, intuitive web interface with alerts, maps, and optional notifications.

---

## 🚀 Features

- 🔔 Real-time alerts for natural disasters (earthquakes, storms, wildfires, etc.)
- 🗺️ Interactive world map with location-based filters
- 📲 Mobile-friendly interface (PWA ready)
- 🌐 Multi-language support (coming soon)
- 🧭 Admin dashboard for NGOs/local authorities (future phase)
- 📡 Data fetched from public sources (USGS, GDACS, NASA, etc.)

---

## 🧱 Tech Stack (MVP Version)

### Backend
- **Python + FastAPI** – API and backend logic
- **Requests / aiohttp** – for fetching live disaster data
- **PostgreSQL** – (optional in later version) for persistent storage
- **Render / Railway** – for cloud deployment

### Frontend
- **HTML/CSS/JS** (basic version)
- **Leaflet.js** – interactive maps
- **React (later)** – for scalable UI components

### Notification (future)
- **Firebase Cloud Messaging (FCM)** for push alerts
- **Email/SMS** (SendGrid/Twilio) for broader reach

---

## 📡 API Sources

| Disaster Type | Source | Format |
|---------------|--------|--------|
| Earthquakes | [USGS](https://earthquake.usgs.gov/fdsnws/event/1/) | JSON |
| Cyclones/Storms | [GDACS](https://www.gdacs.org/xml/) | XML |
| Fires | [NASA FIRMS](https://firms.modaps.eosdis.nasa.gov/) | GeoJSON |
| Volcanoes | [VolcanoDiscovery](https://www.volcanodiscovery.com/) | Scraping/XML |

---

## 📦 Project Structure

```
📁 disaster-alert-system
├── backend
│   └── main.py (FastAPI server)
│   └── fetcher.py (fetches live data)
│   └── utils.py
├── frontend
│   └── index.html
│   └── map.js (Leaflet integration)
│   └── style.css
├── .env (API keys if needed)
├── requirements.txt
└── README.md
```

---

## ⚙️ Setup Instructions

1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/disaster-alert-system.git
   cd disaster-alert-system
   ```

2. **Set up backend:**
   ```bash
   cd backend
   pip install -r requirements.txt
   uvicorn main:app --reload
   ```

3. **Open frontend:**
   - Open `frontend/index.html` in browser

---

## 🎯 Goals for Phase 1 (MVP)

- ✅ Build working backend that fetches live data
- ✅ Display data on map using Leaflet.js
- ✅ Allow filter by disaster type
- ✅ Deploy public version

---

## 🧩 Future Plans

- Mobile app using React Native
- User login + location-based alerts
- Admin dashboard for data input by NGOs
- Machine learning predictions for risk zones

---

## 🤝 Contributing

This project aims to provide real-time safety to vulnerable regions. If you’re a developer, NGO, or designer interested in joining this initiative, feel free to fork and contribute.

---

## 📜 License

MIT License – free to use and modify with attribution.

---

## 🌟 Inspiration

Inspired by global disasters where **information delay costs lives.** This project aims to reduce that gap.

> “Preparedness is the only defense against the unpredictable.”
