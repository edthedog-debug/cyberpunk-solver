# cyberpunk-solver

# Militech Coupler v8.0 - Cyberpunk 2077 Breach Protocol Solver

An automated, mobile-friendly web tool designed to solve the **Breach Protocol (Invasion Protocol)** minigame from *Cyberpunk 2077*. This application allows netrunners to capture the game screen in real-time using their device's camera or upload a picture from their gallery. The built-in geometric OCR engine automatically calibrates, structures the code matrix, separates target sequences, and computes the absolute optimal hacking path using an advanced backtracking algorithm.

## 🚀 Live Demo

You can use the application directly from your smartphone or desktop browser here:
👉 **[Launch Militech Coupler (Live App)](https://edthedog-debug.github.io/cyberpunk-solver/)**

---

## ✨ Features

- **Dual Input Modes:** - **Live Camera Scanning:** Point your phone parallel to your monitor/screen and scan instantly.
  - **Gallery Photo Upload:** Take a picture using your console/PC screenshot tool or phone gallery and upload it.
- **Auto-Calibration Matrix OCR:** Features an elastic geometric clustering algorithm that automatically corrects perspective tilts, ignoring game UI clutter like Daemons or Data Mining icons.
- **Fuzzy Token Matching:** Advanced built-in error correction for common optical misreadings (e.g., auto-corrects `8D` or `B0` to `BD`, `IC` to `1C`, `74` to `7A`).
- **Interactive UI:** The detected code matrix and target sequences populate standard text areas, allowing quick manual adjustments before calculating.
- **Custom Buffer Size:** Supports buffer limitations from 4 up to 8 slots.
- **Cyberpunk 2077 Aesthetic:** Designed with a clean, fully responsive Militech tactical corporate interface.

---

## 🛠️ How to Use

1. **Open the Live App Link** on your smartphone or browser.
2. **Load your Breach Protocol Screen:**
   - Tap **"Subir Foto desde Galería"** to upload an image/screenshot of your matrix.
   - Alternatively, grant camera permissions and tap **"Escanear con Cámara en Vivo"**.
3. **Verify Detected Data:** Ensure the *Matriz de Código* (Code Matrix) and *Se Necesita Secuencia* (Required Sequences) spaces reflect your screen. You can tap and edit them manually if a glare or reflection blurred a specific hex token.
4. **Set Buffer Size:** Adjust the number to match your in-game cyberware buffer capacity.
5. **Calculate:** Tap **"Calcular Ruta de Invasión Óptima"**.
6. **Execute:** Follow the step-by-step sequence displayed under the results panel to unlock maximum rewards.

---

## 🧮 Tech Stack

- **Frontend:** Pure HTML5, CSS3 (CSS Variables, Grid, Responsive Design).
- **OCR Engine:** Modern asynchronous implementation of [Tesseract.js v4](https://github.com/naptha/tesseract.js) (Client-side, no servers or data logging).
- **Solver Core:** Custom JavaScript deterministic backtracking algorithm optimizing for highest sequence completion weight and lowest buffer footprint.

---

## 🔒 Privacy & Performance

All image processing and text recognition are executed **locally inside your web browser**. No photos or data are ever uploaded to external servers, making the solver lightning-fast and entirely offline-capable once loaded.

*Disclaimer: This is an independent open-source fan project. "Cyberpunk 2077" is a registered trademark of CD Projekt Red.*
