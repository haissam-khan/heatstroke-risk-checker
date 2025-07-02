# 🌡️ Heatstroke Risk Checker (熱中症リスクチェック)

A bilingual web app (English / 日本語) that helps workers and field teams assess heatstroke risk based on local weather forecasts and WBGT calculations. Built for internal safety use at Air Liquide Japan, this tool promotes safer work planning during extreme summer heat.

## 🎯 Purpose

In hot and humid environments like Japan's summer season, heat-related illness is a major safety concern. This app helps assess real-time and forecasted risk levels by location, using temperature, humidity, cloud cover, and wind speed to approximate WBGT (Wet Bulb Globe Temperature) values.

## 💡 Features

- 🔁 **Bilingual Support (EN/JA)** — Toggle between English and Japanese UI
- 📍 **Location-Based Search** — Accepts city names or postal codes in Japan
- 🌡️ **WBGT Estimation** — Based on MHLW and JIS B 7922 guidelines
- 📊 **Risk Visualization** — Color-coded gauge and 24-hour forecast table
- ✅ **Safety Tips** — Personalized guidance based on WBGT, cold risk, and rain
- 📱 **Responsive UI** — Works well on desktop and mobile

## 🧠 WBGT Levels & Risk Interpretation

| WBGT (°C) | Risk Level         | Action                                |
|-----------|--------------------|----------------------------------------|
| < 21      | Almost Safe        | Normal hydration                       |
| 21–25     | Caution            | Hydrate consciously, take breaks      |
| 25–28     | Warning            | Avoid strenuous activity               |
| 28–31     | Severe Warning     | Shift work to cooler times             |
| ≥ 31      | Danger             | Avoid outdoor work                     |

_Note: WBGT is estimated and does not include direct solar radiation._

## 🛠️ Tech Stack

- HTML, Tailwind CSS, JavaScript (Vanilla)
- OpenWeatherMap Geocoding + Forecast APIs
- Custom WBGT approximation algorithm
- Fully client-side, no backend

## 🚀 How to Use

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/heatstroke-risk-checker.git
