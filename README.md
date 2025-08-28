# 🕰️ Orienta – Alarm • Stopwatch • Timer • Weather

A sleek, mobile-friendly web application that combines an **Alarm Clock**, **Weather Display**, and device orientation features in a single interface. Built with **HTML**, **CSS**, and **JavaScript**.  

[🌐 Live Demo](https://orienta-app.netlify.app) • [💻 GitHub Repo](https://github.com/Yolisaq/Yolisa_Orienta)

---

## 🚀 Features

### ⏰ Alarm Clock
- 🟢 Set, clear, and snooze alarms.
- Rings even when switching modes.
- Visual indicator for alarm status:
  - 🟢 Alarm Set
  - 🔴 Alarm Cleared
  - ⏰ Ringing!
- ⏱️ Snooze function adds **5 minutes** to the alarm.
- 📳 Vibration support for devices that allow it.

### 🌤️ Weather
- 🌡️ Displays **current weather** with emoji icons.
- Shows **temperature**, **summary**, and **high/low for the day**.
- 📍 Auto-detects your location via Geolocation API.
- 🌆 Option to manually use **Johannesburg coordinates**.
- 🛰️ Weather data provided by **Open-Meteo (free)**.

### 📱 Orientation-Based Mode Switching
- Portrait (↑ or ↓) → Alarm Clock
- Landscape (→ or ←) → Weather
- 🔄 Automatically detects **screen rotation**.
- 📐 Angle readout for debugging: `angle: X°`.

### 🎨 Design
- 🌑 Dark, modern theme with radial gradients.
- ✨ Smooth animations when switching modes.
- 📱 Responsive layout for mobile and desktop.

### 🔊 Audio
- 🔔 Alarm tone: Google Actions Alarm Clock sound
- 🔉 Snooze tone: Short beep
- 🔁 Looping for continuous alarm until cleared.

---

## 🛠️ How to Use

1. **Open [🌐 Orienta App](https://orienta-app.netlify.app)** in a browser.
2. **Set an alarm**:  
   - Tap the alarm time input, select a time, and click **Set Alarm**.
3. **Clear an alarm**:  
   - Click **Clear** to stop the alarm.
4. **Snooze**:  
   - Click **Snooze 5m** to postpone the alarm by 5 minutes.
5. **Check weather**:  
   - Rotate your device to landscape, or click **Refresh** to update.
   - Optionally click **Use JHB** to view Johannesburg weather.

---

## 📂 File Structure
