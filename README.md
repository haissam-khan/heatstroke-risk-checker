# 🌡️ Heatstroke Risk Checker | 熱中症リスクチェック

A bilingual safety tool designed to help field teams, site managers, and contractors in Japan assess heatstroke risk using WBGT (Wet Bulb Globe Temperature), rain, wind chill, and temperature forecasts. Built with legal and operational responsibility in mind — safety isn't optional, it's our duty.

## 🧠 What This Project Does

This web app allows users to input a Japanese city or postal code and receive a 30-hour forecast that includes:
- WBGT-based heat risk levels
- AI-generated safety plans (with or without activity context)
- Bilingual interface (Japanese / English)
- Tips for hydration, breaks, and safe timing of fieldwork

## 🎯 Why It Matters

In Japan, extreme summer heat poses serious risks to outdoor workers. Under both law and company policy, project managers and site leads are responsible for early detection, planning, and documentation to prevent heatstroke incidents.

🔺 **Legal Note (Japanese Law)**  
Employers and site managers are obligated to:
- Detect and report heatstroke cases early  
- Prepare a response procedure and emergency contact system  
- Train relevant personnel on both

**Penalties** include:
- Up to 6 months detention or ¥500,000 fine for individuals
- Up to ¥500,000 fine for corporations

As a project manager at Air Liquide Japan, I built this tool as part of our commitment to safety, legal compliance, and ethical project delivery.

## 🚀 Features

- 🔄 **Bilingual UI** — Switch between English and Japanese
- 📍 **Location-based risk** — Use city or postal code
- 📊 **WBGT gauge** — Live risk level using scientific estimates
- 🧠 **AI-powered safety advice** — Based on Gemini API
- 📝 **Optional activity-specific plans**
- 🌧️ Rain and cold stress indicators
- 📱 Mobile-friendly, single-page app

## 💡 WBGT Levels & Risk Interpretation

| WBGT (°C) | Risk Level         | Action                                |
|-----------|--------------------|----------------------------------------|
| < 21      | Almost Safe        | Normal hydration                       |
| 21–25     | Caution            | Hydrate consciously, take breaks      |
| 25–28     | Warning            | Avoid strenuous activity               |
| 28–31     | Severe Warning     | Shift work to cooler times             |
| ≥ 31      | Danger             | Avoid outdoor work                     |

_Note: WBGT is estimated and does not include direct solar radiation._

## 🛠️ Tech Stack / Tools Used

- HTML / Tailwind CSS / Vanilla JavaScript  
- OpenWeatherMap API (Geocoding + Forecast)  
- Gemini API (for safety planning and activity insights)  
- Custom WBGT estimation logic  
- Legal/standards: MHLW guidelines, JIS B 7922, internal safety rules

## 🌐 Live Demo

👉 [https://khanhaissam.github.io/heatstroke-risk-checker/](https://khanhaissam.github.io/heatstroke-risk-checker/)

## 🧪 How to Run This Project

> No setup needed — just clone and open `index.html` in your browser.

### 🔑 Step 1: Add Your OpenWeatherMap API Key

1. Get a free API key: [https://openweathermap.org/api](https://openweathermap.org/api)  
2. In the HTML file, replace:
```js
const API_KEY = 'YOUR_OPENWEATHERMAP_API_KEY_HERE';

### 🤖 (Optional) Gemini API Setup for AI Advice

1. Sign up at [https://makersuite.google.com/](https://makersuite.google.com/)
2. In the JavaScript, locate the Gemini API fetch section and replace with your own API key:
```js
const apiUrl = "https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-pro:generateContent?key=YOUR_GEMINI_API_KEY";
