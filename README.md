---

# 🚀 Universal Display Controller

A native, ultra-lightweight host application built for secondary PC screens, chassis bar displays, AIO liquid cooler LCDs, and USB hardware monitoring panels. Say goodbye to bloated software—design, drag, drop, and stream live 60 FPS customizable dashboards directly from your web browser.


---

## ✨ Features


* **Native Cross-Platform**: Native binaries for **macOS (Apple Silicon & Intel)**, **Windows**, **Linux**, and **Linux ARM (Raspberry Pi)**.
* **Web-Based Visual Editor**: Modern Canva/Figma-style drag-and-drop UI. No manual pixel coordinate entering required.
* **Responsive Theme Engine**: One-size-fits-all layout engine automatically adapts themes to round AIO coolers, ultra-wide bar displays (32:9), or standard USB screens.
* **Hardware Sensors & Metrics**: Real-time tracking of CPU/GPU temperatures, power usage, fan speeds, memory, battery, and custom HTTP data source APIs.
* **Custom Typography & Templates**: Upload custom `.ttf`/`.otf` fonts, design layered templates, and easily import/export JSON theme packages.

---

## 🖼️ Interface & Key Modules

**1. Live Task & Screen Streaming** Select target USB/secondary display devices, set custom resolutions, output angles (0°/90°/180°/270°), decode FPS, and stream real-time video or dynamic OSDs.

**2. Visual Layer & Widget Editor** Drag, align, and layer text, clocks, system info, circular gauges, bar charts, line graphs, and video backgrounds. Save your canvas layouts as reusable templates with a single click.

**3. Responsive Theme Manager** Manage, preview, and apply theme templates across different canvas dimensions (e.g., 1920×462, 1920×480). Export and share lightweight JSON theme files with the community.

**4. System Metrics & Custom Data Sources** Automatically fetches low-level system sensor data (CPU core temps/wattage, GPU usage, battery status, memory) with support for adding custom REST API endpoints.

**5. Custom Fonts & Media Library** Drag-and-drop file management for custom fonts (`.ttf`/`.otf`), background images, and video clips with real-time typography previews.

---

## 🎬 Showcase & YouTube Demos

Check out real-world hardware rendering and web editing setups in action:

| 📺 Full Video Showcase | 📱 YouTube Shorts Preview |
| --- | --- |
| [[Watch Full Video] Native macOS Setup & Web Editor Guide](https://youtu.be/dyt2z0SCtjo) | [Responsive Layouts & Live Stream](https://youtube.com/shorts/36SOMTpNXqI?feature=share) |

> 💡 **Get More Themes**: Subscribe to our [Channel](https://www.youtube.com/@bdlee/shorts) for weekly open-source theme drops and display setups!

---

## 🛠️ Quick Start

### 1. Download & Run

Download the standalone binary for your OS from the [Releases](https://featherosd.com/) page:

```bash
# macOS / Linux
chmod +x app
./app

# Windows
Double-click app.exe

```

### 2. Access the Web Dashboard

Open your browser and navigate to:
`http://localhost:4137`

## 📟 Supported Devices & Displays

Our engine currently supports out-of-the-box hardware integration for popular USB displays, bar screens, and smart displays via VID/PID auto-matching:

| Device Name | Vendor ID (VID) | Product ID (PID) | Base Resolution | Form Factor / Aspect Ratio |
| :--- | :--- | :--- | :--- | :--- |
| **LIANLI Universal 8.8"** | `0x1CBE` | `0xA088` | 480 × 1920 | Stretched Bar Screen (1:4) |
| **Turzx 8.8"** | `0x1CBE` | `0x0088` | 480 × 1920 | Stretched Bar Screen (1:4) |
| **Thermalright 9.16"** | `0x0416` | `0x5408` | 1920 × 462 | Ultrawide Bar Screen (~32:9) |
| **Turning-5.2 Inch** | `0x1CBE` | `0x0050` | 720 × 1280 | Vertical Smart Screen (9:16) |
| **TurningSmart3.5** | `0x1A86` | `0x5722` | 320 × 480 | Mini USB Sensor Screen (2:3) |

> 💡 **Custom Devices**: You can easily add, edit, or map any new USB display by entering its `VID` and `PID` directly through the Web UI (`USB Devices` tab).

---

## 🤝 Community & Support

If you find this project useful, give it a **⭐ Star** on GitHub!

* **Share Themes**: Submit your custom JSON layouts to the `themes/` directory to share with the community.
* **Device Support**: Missing support for a specific USB screen or cooler? Open an [Issue](https://github.com/featherosd/featherosd/issues) with your hardware VID/PID.
