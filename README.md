# ======================= SkyTrack – Weather Forecast App ===============================

SkyTrack is a clean and lightweight weather forecast application built using **Vanilla JavaScript**, **Tailwind CSS**, and the **WeatherAPI**.  
The app shows real-time weather, of current location, a 5-day forecast, and keeps track of your recent searched cities using localStorage.

## Live Demo

_(not available right now)_

## Features ===============================================================

### ✔ Current Weather

- Live temperature
- Weather condition
- “Feels like” temperature
- Humidity & Wind speed
- Supports °C / °F toggle

### ✔ 5-Day Forecast

- Clean date format (Day + Month only)
- Weather icons from API
- Max & Min temperatures

### ✔ Recent Search History

- Saves recent cities using localStorage
- Highlights the selected city
- Current location always stays at the first position
- Maintains order even after page refresh

### ✔ Dynamic Background

Background updates based on the latest weather:  
• Sunny • Cloudy • Rainy • Snow • Mist • Thunder • Night mode

### ✔ Responsive UI

Optimized for:

- Desktop
- iPad Mini
- iPhone SE

Everything stays in place without breaking your original design.

---

## Project Structure ======================================================

WEATHER FORECAST PROJECT
│
│── src/
│ ├── assets/
│ │ └── images/
│ │ ├── cloudy.jpg
│ │ ├── default.jpg
│ │ ├── mist.jpg
│ │ ├── night.jpg
│ │ ├── rain.jpg
│ │ ├── snow.jpg
│ │ ├── sunny.jpg
│ │ └── thunder.jpg
│ │
│ ├── index.html
│ ├── input.css
│ ├── output.css
│ └── script.js
│
├── package.json
├── package-lock.json
├── .gitignore
└── README.md

## Technologies Used ======================================================

- HTML5
- Tailwind CSS
- JavaScript (Vanilla ES6)
- WeatherAPI
- LocalStorage API

---

## How to Run Locally =====================================================

1. Clone the repository:
   git clone https://github.com/sartaza123/WEATHER-Forecast-Application-JavaScript-.git

2. Move into the project folder:
   cd WEATHER-Forecast-Application-JavaScript-

3. Run [ npm install ] This will recreate node_modules.

4. Open index.html directly in your browser (no server needed).

5. (Optional) Add your own WeatherAPI key in script.js:
   const url = `https://api.weatherapi.com/v1/...key=YOUR_API_KEY`;

## IMPORTANT ====

After deleting node_modules, do NOT run:
[ npm start ] or [ npx tailwindcss -i ./src/input.css -o ./src/output.css --watch ]

### How It Works ==========================================================

- When the page loads, the browser's GPS detects your current location and fetches the weather automatically (using Geolocation).
- Weather data is fetched using JavaScript’s fetch() and displayed instantly.
- When you search for a city for the weather details:
  - If ssearched city is not in history → it gets added to localStorage.
  - If it exists in localStorage → It only highlight updates.
  - The UI updates and background changes based on the weather.
- Recent searches persist even after refreshing the page.

## 🙋‍♂️ Author ==============================================================

**Md Sartaz Ansari**

If you like the project, please ⭐ the repository on GitHub.
