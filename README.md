# CleanCity Premium 🌍🏙️

**CleanCity Premium** is a gamified web application designed to encourage citizens to report uncollected waste and help maintain a cleaner environment. Users can take photos of garbage, get it analyzed by AI, and earn points to climb the city leaderboard!

## 🚀 Key Features

- **Waste Reporting & AI Analysis**: Upload photos via Camera or Gallery. The app uses **TensorFlow.js (MobileNet)** to verify if the uploaded image contains waste before submission.
- **Interactive Mapping**: Powered by **Leaflet.js**, users can pinpoint exactly where the waste is located and view all reported areas on an interactive city map.
- **Gamification & Leaderboard**: Earn points for successfully reported and resolved waste. Climb the ranks from *Rookie* to *Hero* on the **City Heroes Leaderboard**.
- **Admin Dashboard**: Dedicated `admin.html` interface for authorities to review, reject, or mark complaints as resolved and upload proof-of-cleanup imagery.
- **Accessibility & UX**:
  - Full **Dark Mode / Light Mode** support with smooth glassmorphism UI.
  - Text-to-Speech (TTS) integration using the **ElevenLabs API** for greeting users and giving feedback.
- **Cloud Infrastructure**: Fully robust backend powered by **Firebase** (Authentication & Realtime Database) and **ImgBB** for image hosting.

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3 (Vanilla / Custom Properties), Vanilla JavaScript (ES Modules)
- **Backend / Database**: Firebase Version 9 (Authentication, Realtime DB)
- **Mapping**: Leaflet JS
- **Machine Learning**: TensorFlow.js pre-trained MobileNet model
- **APIs**: ImgBB (Image Storage), ElevenLabs (Text-to-Speech), OpenStreetMap Nominatim (Reverse Geocoding)

## 💻 Local Setup Instructions

**IMPORTANT**: Because this app uses modern ES Modules (`<script type="module">`), it **cannot** be opened directly by double-clicking the `index.html` file (the `file:///` protocol will block the scripts due to CORS security policies, resulting in a blank screen).

You **must** run it through a local HTTP server.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/basantnema31/clean-city.git
   cd clean-city
   ```

2. **Serve the project locally:**
   Using Node.js & `http-server`:
   ```bash
   npx http-server -p 8080
   ```
   *Alternatively, you can use Python's built-in server:*
   ```bash
   python -m http.server 8080
   ```

3. **Open the App:**
   Open your browser and navigate to:
   ```
   http://localhost:8080/index.html
   ```

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Let's build a greener future together. 🌱