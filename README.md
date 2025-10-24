# Live Weather App

A modern, responsive weather application that provides real-time weather information for any city worldwide.

## Features

- **Real-time Weather Data**: Get current weather conditions for any city
- **6-Day Forecast**: View upcoming weather predictions
- **Location-based Weather**: Automatically detect and display weather for your current location
- **Unit Toggle**: Switch between Celsius and Fahrenheit
- **Auto-refresh**: Weather data updates automatically every 15 minutes
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI**: Clean, intuitive interface with weather icons and animations

## Screenshots
<img width="1001" height="948" alt="image" src="https://github.com/user-attachments/assets/c9b9f12f-e000-4b40-bd10-6c46f90d5d08" />


<img width="1329" height="946" alt="Screenshot 2025-10-24 195319" src="https://github.com/user-attachments/assets/a65bbd30-7423-46b3-9c1a-3e80b7c165a4" />


The app displays:
- Current temperature and weather conditions
- Feels-like temperature, humidity, wind speed, and UV index
- 6-day weather forecast with icons
- Real-time date and time updates

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for weather data

### Installation

1. Clone or download this repository
2. Open `index.html` in your web browser
3. That's it! No additional setup required.

### Running the App

Simply open the `index.html` file in any modern web browser:

```bash
# On Windows
start index.html

# On macOS
open index.html

# On Linux
xdg-open index.html
```

Or double-click the `index.html` file in your file explorer.

## Usage

### Search for Weather
1. Type a city name in the search bar
2. Press Enter or click the search button
3. View the current weather and forecast

### Use Current Location
1. Click the location button (📍) in the top-right corner
2. Allow location access when prompted
3. Your local weather will be displayed

### Toggle Temperature Units
- Click the °C or °F buttons to switch between Celsius and Fahrenheit

### Refresh Data
- Click the refresh button (🔄) to manually update weather data
- Data automatically refreshes every 15 minutes

## Technical Details

### Built With
- **HTML5**: Structure and semantic markup
- **CSS3**: Styling with modern features like Grid, Flexbox, and animations
- **Vanilla JavaScript**: Dynamic functionality and API integration
- **OpenWeatherMap API**: Weather data source

### File Structure
```
live-weather-app/
├── index.html          # Main HTML file
├── style.css           # Stylesheet
├── script.js           # JavaScript functionality
└── README.md           # This file
```

### API Integration
The app uses the OpenWeatherMap API to fetch weather data. The API provides:
- Current weather conditions
- 5-day/3-hour forecast data
- Weather icons and descriptions

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Features in Detail

### Weather Information Displayed
- **Current Temperature**: Real-time temperature reading
- **Weather Description**: Clear description of current conditions
- **Feels Like**: Apparent temperature based on humidity and wind
- **Humidity**: Current humidity percentage
- **Wind Speed**: Wind speed in km/h
- **UV Index**: Simulated UV index based on temperature
- **6-Day Forecast**: Daily weather predictions with icons

### User Interface Features
- **Loading States**: Smooth loading animations while fetching data
- **Error Handling**: User-friendly error messages for failed requests
- **Responsive Design**: Adapts to different screen sizes
- **Modern Styling**: Glass-morphism effects and smooth animations
- **Accessibility**: Proper contrast ratios and semantic HTML

## Customization

### Changing the Default City
Edit the `initApp()` function in `script.js` to change the default city:

```javascript
// Change 'London' to your preferred default city
getWeatherByCity('YourCity');
```

### Modifying Refresh Interval
Change the auto-refresh interval in the `startAutoRefresh()` function:

```javascript
// Change 900000 (15 minutes) to your preferred interval in milliseconds
refreshInterval = setInterval(() => {
    refreshWeather();
}, 900000); // 15 minutes = 900000ms
```

### Styling Customization
Modify the CSS custom properties in `style.css` to change the color scheme:

```css
:root {
    --primary: #4361ee;        /* Primary color */
    --secondary: #3a0ca3;      /* Secondary color */
    --accent: #4cc9f0;         /* Accent color */
    /* ... other variables */
}
```

## Troubleshooting

### Common Issues

**Weather data not loading:**
- Check your internet connection
- Ensure the city name is spelled correctly
- Try refreshing the page

**Location not working:**
- Make sure location services are enabled in your browser
- Grant location permission when prompted
- Check if your browser supports geolocation

**App not displaying correctly:**
- Ensure you're using a modern browser
- Clear your browser cache
- Check if JavaScript is enabled

## Contributing

Feel free to contribute to this project by:
1. Reporting bugs
2. Suggesting new features
3. Submitting pull requests
4. Improving documentation

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Weather data provided by [OpenWeatherMap](https://openweathermap.org/)
- Icons from [Boxicons](https://boxicons.com/)
- Fonts from [Google Fonts](https://fonts.google.com/)

---

**Enjoy using the Live Weather App!** 🌤️
