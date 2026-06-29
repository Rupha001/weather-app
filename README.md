# Weather App

A Flutter weather application that displays real-time weather data using the [OpenWeatherMap API](https://openweathermap.org/api).

## Features

- Current temperature, sky condition, and weather icon
- Hourly forecast (next 5 hours)
- Additional info: humidity, wind speed, and pressure
- Dark theme with glassmorphism card effect
- Pull-to-refresh support

## Screenshots

> _Add screenshots here after running the app_

## Getting Started

### Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (3.x or higher)
- An [OpenWeatherMap API key](https://openweathermap.org/api) (free tier works)

### Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/YOUR_USERNAME/weather-app.git
   cd weather-app
   ```

2. **Add your API key**
   ```bash
   cp lib/secrets.example.dart lib/secrets.dart
   ```
   Open `lib/secrets.dart` and replace `YOUR_OPENWEATHER_API_KEY` with your actual key.

3. **Install dependencies**
   ```bash
   flutter pub get
   ```

4. **Run the app**
   ```bash
   flutter run
   ```

## Project Structure

```
lib/
├── main.dart                 # App entry point
├── weather_screen.dart       # Main screen with weather data
├── hourly_forecast_item.dart # Hourly forecast card widget
├── additional_info_item.dart # Humidity/wind/pressure widget
└── secrets.example.dart      # API key template (copy to secrets.dart)
```

## Tech Stack

- **Flutter** — UI framework
- **Dart** — Programming language
- **http** — REST API calls
- **intl** — Date/time formatting
- **OpenWeatherMap API** — Weather data source

## Security Note

`lib/secrets.dart` is listed in `.gitignore` and will never be committed. Always use `secrets.example.dart` as the template.
