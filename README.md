# 🔥 Trailer Diesel Heater Web Controller (Zero-Bloat BLE App)

A clean, single-file **Web Bluetooth** controller for **VEVOR 8kW (CY5004)** and compatible 12V/24V Chinese Bluetooth diesel air heaters (`ABBA` / `Chuangli` `0xFFF0` & `0xFFE0` BLE boards).

Built to replace sideloaded third-party APKs with a fast, transparent, zero-tracking interface that runs directly in your browser—complete with 7-day hardware scheduling, fuel burn forecasting, 7-day overnight weather lows, and carbon de-soot tracking.

### 🚀 **[Launch Live Web Controller](https://andrewmeades.github.io/vevor-heater-controller/)**
📺 **[Watch the Full Enclosed Trailer Install & Setup Video on YouTube](https://youtu.be/q9EuvBHhfc4)**

---

## ✨ Key Features

* **Zero Sideloaded Bloatware:** Runs entirely in a single static `index.html` file using Web Bluetooth. No accounts, no background tracking, no sketchy permissions.
* **Live Heater Telemetry:** Real-time Supply Voltage (with 12V/24V maintainer float & low-battery warnings), Ambient Cabin/Trailer Temp, Cast-Aluminum Heat Exchanger Temp, and `E-02` through `E-CO` fault decoding.
* **Reliable 7-Day Hardware Timer:** Syncs your phone's clock to the heater's onboard chip and writes 20-byte chunked BLE schedules (plus a 1-tap **Clear & Disable All Timers** wipe). **Your phone does not need to be in range for scheduled 5:00 AM pre-heats to run.**
* **Diesel Tank Estimator & Refill Forecast:** Calibrated for the 5.0 L (1.32 gal) CY5004 sight glass—or any custom tank size—with per-day fuel projections across your scheduled runs.
* **7-Day Overnight Freeze Forecast:** Optional 1-tap lookup (via Open-Meteo) displays upcoming overnight lows right beside each day's schedule toggle.
* **Chamber Carbon / De-Soot Tracker:** Logs low-idle hours (`Lvl 1–3` / Thermostat idle) and includes a 1-tap **15-Minute Max Burn** timer to keep the glow-plug mesh clean.
* **One-Tap `°C / °F` Toggle:** Instantly switches temperatures (`°C` ↔ `°F`) and fuel volumes (`Liters` ↔ `US Gallons`) across the entire app and user guide.

---

## 📱 Compatible Browsers & Devices

Because this controller uses the **Web Bluetooth API** to talk directly to your heater's radio:

* **Android Phones & Tablets:** Works out of the box in **Google Chrome** or **Microsoft Edge**. *(Tap `📲 APP` or Chrome's `⋮ → Add to Home screen` to install it like a native full-screen app).*
* **Windows / macOS / Linux / Chromebook:** Works out of the box in **Google Chrome**, **Edge**, or **Brave**.
* **iPhone / iPad (iOS):** Apple blocks Web Bluetooth inside Safari. To use this controller on an iPhone, install the free **[Bluefy – Web BLE Browser](https://apps.apple.com/us/app/bluefy-web-ble-browser/id1492822055)** from the Apple App Store and paste the live controller URL inside Bluefy.

---

## 🛠️ Supported Heater Hardware

Designed and tested on the **VEVOR 8kW 12V Bluetooth Diesel Air Heater (Model CY5004)** and compatible controllers broadcasting:
* **BLE Service UUIDs:** `0xFFF0` or `0xFFE0` (typically advertising as `HeaterXXXX`, `BT_XXXX`, or `@XXXX`)
* **Protocol Header:** `0xBAAB` (TX) / `0xABBA` (RX)

---

## ⚠️ Safety Notice

* **Never Cut 12V Power While Hot:** Always shut down using the controller's **STOP** button and allow the 3–5 minute **COOLING** fan cycle to bring the heat exchanger below ~55°C (131°F) before disconnecting battery power.
* **Exhaust & Carbon Monoxide (CO):** Ensure all exhaust piping is routed outside with gas-tight clamps and proper clearance from combustible materials (such as a stainless steel turret floor plate). Always use an independent, battery-powered UL/CSA-listed Carbon Monoxide alarm in any enclosed trailer, cabin, or vehicle.
* **Use at Your Own Risk:** This is an independent community project not affiliated with VEVOR. Provided "as-is" under the MIT License.
