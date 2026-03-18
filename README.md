# SkySpy - A Socially Anxious Weather App
An app that watches the clouds so you don't have to make eye contact with the sun. Real-time data for people who plan their life around avoiding rain.
A sleek, responsive weather application built with vanilla JavaScript that displays real-time weather data for any location worldwide. The app features automatic geolocation detection, manual city search, and a modern gradient UI.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## Features

- **Automatic Location Detection** -- Uses the browser's Geolocation API to fetch weather for your current position on load.
- **City Search** -- Search for any city worldwide using the input field or by pressing Enter.
- **Current Conditions** -- Displays temperature, weather description, humidity, and wind speed.
- **Daily Phase Temperatures** -- Shows morning, day, evening, and night temperatures at a glance.
- **Dynamic Backgrounds** -- Background image updates dynamically based on the searched city via Unsplash.
- **Hover Animations** -- Smooth CSS transitions and scaling effects on interactive elements.
- **Clean, Modern UI** -- Dark-themed card layout with a gradient overlay and the Montserrat typeface.

---

## Demo

Simply open `index.html` in your browser. The app will request location access and immediately display the weather for your current area.

---

## Tech Stack

| Layer     | Technology                                                  |
|-----------|-------------------------------------------------------------|
| Markup    | HTML5                                                       |
| Styling   | CSS3 (Flexbox, gradients, transitions, Google Fonts)        |
| Logic     | Vanilla JavaScript (ES6 Fetch API, Geolocation API)         |
| Icons     | [Font Awesome](https://fontawesome.com/)                    |
| API       | [OpenWeatherMap](https://openweathermap.org/api) (Current Weather & One Call) |
| Images    | [Unsplash Source](https://unsplash.com/) (dynamic backgrounds) |

---

## Project Structure

```
weather-app/
├── index.html    # Main HTML page
├── style.css     # All styles (layout, colors, animations)
├── script.js     # Application logic & API calls
└── README.md     # Project documentation
```

---

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Edge, Safari)
- An internet connection (required for API calls and external assets)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/this-ved-dev/weather-app.git
   cd weather-app
   ```

2. **Open the app**

   Open `index.html` directly in your browser, or use a local development server:

   ```bash
   # Using Python
   python3 -m http.server 8080

   # Using Node.js (http-server)
   npx http-server -p 8080
   ```

3. **Allow location access** when prompted by the browser to see weather for your current location.

---

## Usage

1. On launch, the app automatically detects your location and displays the current weather.
2. To check weather for a different city, type the city name in the search field and press **Enter** or click **Change Location**.
3. The background image, temperature, humidity, wind speed, and phase-wise temperatures update instantly.

---

## API Reference

This app uses the [OpenWeatherMap API](https://openweathermap.org/api):

- **Current Weather Data** -- Fetches basic weather info and coordinates for a given city.
- **One Call API** -- Retrieves detailed current and daily forecast data using latitude and longitude.

> To use your own API key, replace the `key` variable at the top of `script.js` with your OpenWeatherMap API key.

---

## Customization

- **API Key** -- Update the `key` constant in `script.js` with your own OpenWeatherMap API key.
- **Units** -- Change `units=metric` to `units=imperial` in the API URLs within `script.js` to switch to Fahrenheit.
- **Styling** -- Modify `style.css` to adjust colors, fonts, spacing, and animations.

---

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/my-feature`)
3. Commit your changes (`git commit -m "Add my feature"`)
4. Push to the branch (`git push origin feature/my-feature`)
5. Open a Pull Request

---

## License

This project is open source and available for personal and educational use.

---

## Acknowledgements

- [OpenWeatherMap](https://openweathermap.org/) for the weather data API
- [Unsplash](https://unsplash.com/) for dynamic background images
- [Font Awesome](https://fontawesome.com/) for weather and location icons
- [Google Fonts](https://fonts.google.com/) for the Montserrat typeface
