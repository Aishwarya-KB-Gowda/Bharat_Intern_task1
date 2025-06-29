
# **🌦️ Geo-Weather Application**

A responsive weather application that fetches real-time weather information based on your **current location** using browser Geolocation, or through **manual city search**. Built using **HTML, CSS, Bootstrap, and Vanilla JavaScript**, this project highlights frontend API integration and dynamic DOM updates.

---

## **📌 Features**

✅ Automatically detects user's location using browser's **Geolocation API**
✅ Reverse geocoding with **OpenWeather Geo API** to get city name from coordinates
✅ Displays real-time weather details fetched from **WeatherAPI.com**
✅ Manual location search to check weather for any city worldwide
✅ Responsive and user-friendly design using **Bootstrap**
✅ Displays temperature, humidity, cloud percentage, wind details, UV index, etc.
✅ Live date, time, and day shown dynamically
✅ Clean UI with blur effect removed after location detection

---

## **🚀 Project Demo**

✔️ On page load, the app asks for location access
✔️ Displays weather information for current location
✔️ You can search any other location manually
✔️ All weather parameters update dynamically in the UI

---

## **🛠️ Tech Stack**

* **HTML5** — Structure of the application
* **CSS3** — Custom styling
* **Bootstrap 4** — Responsive design
* **JavaScript (Vanilla)** — API integration, DOM manipulation, logic
* **OpenWeather Geo API** — Reverse geocoding (coordinates to location)
* **WeatherAPI.com** — Fetching weather data
* **FontAwesome** — Icons
* **jQuery (Loaded but not actively used)**

---

## **📂 Project Structure**

```
├── index.html           # Main webpage structure
├── styles/
│   └── style.css        # Custom CSS for styling
├── images/
│   └── ai.png           # Image displayed in weather card
├── src/
│   ├── script.js        # Core logic: Geolocation, API calls, weather display
│   └── setdates.js      # Logic to show live date, time, and day
```

---

## **⚡ How the Application Works**

### 🌍 **Geolocation Detection**

* On page load, calls `getLocation()`
* Uses `navigator.geolocation` to fetch latitude & longitude
* Calls `getName()` to convert coordinates to city name using OpenWeather Geo API

### 🌤️ **Fetching Weather Data**

* Calls `fetchData(location)` with city name
* Fetches real-time weather using **WeatherAPI.com**
* Updates DOM with:

  * Temperature
  * Feels-like temperature
  * Location & Region
  * Weather conditions (e.g., Sunny, Cloudy)
  * Cloud cover, Humidity, Wind speed, Pressure, UV index, etc.

### 🔎 **Manual Location Search**

* User can enter a city name
* Clicking search icon triggers `findWeather()`
* Weather data fetched for entered city

### 🕒 **Live Date & Time**

* `setdates.js` updates the top bar with current time, day, and full date
---

## **📥 Setup Instructions (For Local Testing)**

1. Clone the repository
2. Replace API keys in `script.js` with your own valid keys:

   * **OpenWeather Geo API** key
   * **WeatherAPI.com** key
3. Open `index.html` in your browser
4. Allow location access to see current location weather

---

## **🔑 Sample API Resources**

* [WeatherAPI.com — Current Weather Data](https://www.weatherapi.com/)
* [OpenWeather — Reverse Geocoding API](https://openweathermap.org/api/geocoding-api)

---

## **🧑‍💻 Author**

**Aishwarya K B** — Frontend Developer passionate about building interactive and real-time web applications.

