# Weather App

A simple web-based Weather App that allows users to fetch and display real-time weather information by entering a city name. The app utilizes the OpenWeather API to retrieve weather details such as temperature, humidity, and weather conditions.

## Features
- Fetches real-time weather data using OpenWeather API.
- Displays city name, temperature (°C), humidity, and weather conditions.
- Error handling for invalid city names and incorrect API keys.
- Simple and user-friendly interface.

## Technologies Used
- **HTML** – Structure of the web page.
- **CSS** – Styling the application.
- **JavaScript** – Fetching and displaying data dynamically.
- **OpenWeather API** – Retrieves real-time weather data.

## Installation & Usage
### 1️⃣ Get an API Key from OpenWeather
1. Go to [OpenWeather](https://home.openweathermap.org/users/sign_up) and create an account.
2. After signing in, navigate to the [API Keys](https://home.openweathermap.org/api_keys) section.
3. Copy your generated API key.

### 2️⃣ Update the API Key in the Code
1. Open the **weather.html** file.
2. Locate this line in the JavaScript code:
   ```js
   let response = await fetch(`https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=YOUR_API_KEY&units=metric`);
   ```
3. Replace **`YOUR_API_KEY`** with your actual API key.

### 3️⃣ Run the App
1. Save the file.
2. Open **weather.html** in a browser.
3. Enter a city name and click the "Get Weather" button.

## Project Structure
```
/weather-app/
│-- index.html
│-- style.css  (optional styling)
│-- script.js  (weather logic)
│-- README.md  (project documentation)
```

## Code Explanation
### HTML:
- Provides input field for city name and a button to fetch weather details.
- Displays weather results dynamically.

### JavaScript:
- Listens for button clicks and fetches data using **fetch()** from OpenWeather API.
- Parses the JSON response and displays temperature, humidity, and weather description.
- Handles errors (e.g., invalid city names or API key issues).

## Example API Request
```sh
https://api.openweathermap.org/data/2.5/weather?q=London&appid=YOUR_API_KEY&units=metric
```

## Troubleshooting
- **401 Unauthorized:** Invalid API Key → Double-check and regenerate a key if needed.
- **404 Not Found:** City name is incorrect → Try entering a valid city.
- **CORS Issues:** If the request fails, try using a proxy or a backend server.

## Future Enhancements
- Add background images based on weather conditions.
- Implement a 5-day weather forecast.
- Improve UI with CSS animations.

## License
This project is open-source and free to use. Feel free to modify and improve it!

