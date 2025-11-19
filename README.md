📡 NetScope - Professional RF Network Design Tool
A powerful, browser-based WiFi network planning and RF propagation modeling tool for designing enterprise wireless networks. Plan your WiFi coverage with real-time heatmaps, wall attenuation modeling, and comprehensive AP placement analysis.

![NetScope Interface](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

🚀 Try NetScope Now - No Download Required!
<strong>➡️ <a href="https://wolfkyd1.github.io/NetScope/">Launch NetScope</a> ⬅️</strong>
Use NetScope directly in your browser - no installation, no setup, no hassle!

✨ Features
🗺️ Floor Plan Integration

Upload floor plans as images (PNG, JPG) or PDF files
Automatic PDF-to-image conversion
Precise scale calibration tool for accurate measurements
Pan and zoom controls for detailed planning

📶 Access Point Management

Massive device library with 194 pre-configured devices from 14 major brands:
🏢 Enterprise Brands:

Aruba (7 models) - AP-325, AP-515, AP-555, AP-635, AP-655, AP-505H, AP-387
Cisco Meraki (10 models) - MR36, MR46, MR56, MR57, MR86, MR76, MR86E, MR20, MX67W, MX68W
Ruckus (12 models) - R350, R550, R650, R750, R850, R770, T350c, T750, H350, H550, R320, R510
Juniper Mist (8 models) - AP33, AP34, AP43, AP44, AP45, AP63, AP12, AP21
Fortinet (10 models) - FAP-231F, FAP-431F, FAP-433F, FAP-831F, FAP-234F, FAP-234G, FAP-221E, FAP-423E, FAP-231G, FAP-221C
Extreme Networks (10 models) - AP4000, AP410C, AP305C, AP3000, AP4000U, AP302W, AP3965e, AP4000E, AP122, AP250

📊 SMB Brands:

Ubiquiti (33 models) - UniFi 6, UniFi 7, UniFi AC series, Dream Machine series, AmpliFi series
TP-Link (15 models) - EAP series APs, Archer routers, Omada series
Grandstream (9 models) - GWN7630LR, GWN7660, GWN7664, GWN7605, GWN7610, GWN7602, GWN7000/7001 Routers
MikroTik (10 models) - cAP ac, wAP ac, cAP XL ac, Audience, BaseBox 5, SXTsq 5 ac, hAP series
Cambium Networks (12 models) - XV3-8, XV2-2, X4-8, e600, e700, cnPilot series, ePMP series
Netgear Business (12 models) - WAX series, Orbi Pro
EnGenius (10 models) - EWS377AP, EWS357AP, ECW series
Zyxel (10 models) - WAX650S, WAX640S, NWA210AX, WAX610D series

🏠 Consumer Brands:

ASUS (15 models) - ROG Gaming series, ZenWiFi Mesh, RT-AX series
Netgear Consumer (12 models) - Nighthawk series, Orbi Mesh
Linksys (12 models) - Velop Mesh, Gaming routers, MX/EA series
D-Link (10 models) - DIR-X series, COVR Mesh, Business APs


Smart Device Search & Filtering:

🔍 Real-time search by model name or type
📋 Filter by vendor dropdown (14 vendors)
📊 Live device counter showing matches
📡 Visual icons (AP vs Router indicators)
⚡ Instant results as you type


Device Management:

Drag-and-drop AP placement
Real-time signal coverage visualization
AP duplication for quick deployment
Configurable AP settings:

Transmit power (2.4 GHz & 5 GHz)
Channel assignment
Antenna type (omnidirectional/directional)
Antenna orientation
Mounting height
SSID configuration





🧱 Wall & Obstacle Modeling

Draw walls with click-to-place interface
Smart wall snapping for room creation
Snap-to-wall endpoint feature for precise room closures
Material-based attenuation modeling:

Glass (3 dB)
Wood (5 dB)
Drywall (8 dB)
Concrete (12 dB)
Brick (15 dB)
Metal/Elevator Shafts (20 dB)


Automatic room detection with perimeter-first algorithm
Building area calculation
Editable wall properties
Visual wall edit points

🔥 RF Propagation & Heatmaps

Real-time signal strength heatmaps
Free Space Path Loss (FSPL) calculations
Wall attenuation modeling
Multiple resolution settings (Low/Medium/High)
Adjustable heatmap opacity
Coverage circles visualization
Signal strength at any point (click-to-measure)
Directional antenna pattern modeling

👥 Client Simulation

Simulate 10-200 WiFi clients
Automatic AP association
Client density heatmaps
Smart client placement (inside rooms only)
Real-time speed estimates based on RSSI:

WiFi link speed calculation (up to 1.2 Gbps)
Download/upload bottleneck analysis
Per-client signal strength visualization
Internet speed impact modeling



📊 Analysis Tools

Auto-Channel Planning: Automatically assigns non-overlapping channels to minimize interference
Interference Detection: Visualize co-channel and adjacent-channel interference
Coverage Statistics: Real-time coverage percentage calculations (>-65dBm threshold)
Room Analysis: Automatic room detection with area calculations in sq ft
Measurement Tool: Click-to-measure distances in feet with visual indicators
Signal Analysis: Point-and-click signal strength analysis from all APs
Building Statistics: Total building area tracking

📤 Export Capabilities

PDF Reports including:

Project summary with statistics
AP configuration details (position, power, channels)
Coverage heatmap visualization
Room listings with areas
Device type indicators (AP/Router)
Date/time stamps


PNG Heatmap Export: High-resolution coverage maps
JSON Project Files: Save and load complete projects with all settings


🚀 Getting Started
Option 1: Use Online (Recommended)
Simply visit: https://wolfkyd1.github.io/NetScope/
No installation required! Works in any modern browser.
Option 2: Run Locally

Clone the repository:

bash   git clone https://github.com/wolfkyd1/NetScope.git
   cd NetScope
```

2. **Open in browser:**
   - Simply open `index.html` in any modern web browser
   - No build process or server required!

### Quick Start Guide

1. **Upload Floor Plan** 📷
   - Click the "Upload" button in the left toolbar
   - Select an image or PDF of your floor plan

2. **Set Scale** 📏
   - Click the "Scale" tool
   - Click two points on the floor plan with a known distance
   - Enter the actual distance in feet

3. **Add Access Points** 📡
   - Click "Add AP" in the toolbar
   - Use the search box to find your device (e.g., type "U6" or "Meraki")
   - Or filter by vendor using the dropdown
   - Click on your device model
   - Click on the floor plan to place the AP

4. **Draw Walls** 🧱
   - Click the "Wall" tool
   - Click to place points along walls
   - Walls snap to existing walls for easy room creation
   - Double-click or press ESC to finish
   - Select wall material type when prompted

5. **View Coverage** 🔥
   - Coverage heatmap updates automatically
   - Toggle heatmap visibility in bottom-left controls
   - Adjust opacity and resolution as needed
   - Enable coverage circles for visual range indicators

6. **Simulate Clients** 👥
   - Set client count in the right panel (10-200)
   - Click "Simulate Clients"
   - View client connections and density
   - Enable "Show Client Density" for density heatmap

7. **Export Results** 💾
   - Click "Export PDF" for comprehensive reports
   - Click "Export Heatmap" for PNG coverage maps
   - Click "Save" to save project as JSON

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `V` | Select tool |
| `A` | Add Access Point |
| `W` | Draw Wall |
| `Ctrl+Z` | Undo / Remove last wall point |
| `Backspace` | Remove last wall point (during wall drawing) |
| `ESC` | Cancel current action |
| `Delete` | Delete selected object |
| `Space + Drag` | Pan canvas |
| `Mouse Wheel` | Zoom in/out |
| `Ctrl+S` | Save project |

---

## 🎯 Device Library Features

### Search Capabilities
- **Instant Search**: Type any part of a model name or vendor name
  - Example: "U6" finds all Ubiquiti U6 models
  - Example: "Meraki" shows all Cisco Meraki devices
  - Example: "router" filters all router models

### Vendor Filtering
- Quick access to all 14 vendors via dropdown
- See device count per vendor
- Combine search with vendor filter for precise results

### Device Information Displayed
- Model name with type indicator (AP/Router)
- Radio specifications (2.4 GHz and 5 GHz TX power)
- Antenna type and gain
- Beamwidth for directional antennas

---

## 🛠️ Technologies Used

- **[Konva.js](https://konvajs.org/)** - Canvas rendering and object management
- **[Three.js](https://threejs.org/)** - 3D visualization capabilities
- **[jsPDF](https://github.com/parallax/jsPDF)** - PDF generation
- **[PDF.js](https://mozilla.github.io/pdf.js/)** - PDF floor plan rendering
- **[FileSaver.js](https://github.com/eligrey/FileSaver.js/)** - File download functionality
- **[Feather Icons](https://feathericons.com/)** - Beautiful icon set
- **Vanilla JavaScript** - No framework dependencies!

---

## 📐 RF Propagation Model

NetScope uses industry-standard RF propagation calculations:

### Free Space Path Loss (FSPL)
```
FSPL (dB) = 20×log₁₀(d) + 20×log₁₀(f) - 27.55
```

Where:
- `d` = distance in feet
- `f` = frequency in MHz

### Received Signal Strength (RSSI)
```
RSSI = TX_Power + Antenna_Gain - FSPL - Wall_Attenuation
```

### Directional Antenna Pattern
- Main lobe: Full gain within beamwidth
- Side lobes: Up to 20 dB reduction outside beamwidth
- Adjustable antenna orientation (0-359°)

### Signal Quality Thresholds
- **Excellent**: > -50 dBm (1.2 Gbps WiFi 6/6E)
- **Good**: -50 to -65 dBm (600-866 Mbps)
- **Fair**: -65 to -80 dBm (200-400 Mbps)
- **Poor**: < -80 dBm (< 100 Mbps)

---

## 📋 Project Structure
```
netscope/
├── index.html          # Main application file (all-in-one)
├── README.md           # This file
├── LICENSE             # MIT License
└── examples/           # Example projects (coming soon)
    ├── office.json
    ├── warehouse.json
    └── retail.json

🎯 Use Cases

Enterprise WiFi Planning: Design optimal AP placement for offices and campuses
Warehouse Networks: Plan coverage for large industrial spaces
Retail Deployments: Ensure coverage in customer areas
Venue WiFi: Design networks for stadiums, conference centers, hotels
Education: Network planning for schools and universities
Healthcare: RF planning for hospitals with strict coverage requirements
IoT Deployments: Plan coverage for IoT device connectivity
Multi-Vendor Comparisons: Compare coverage from 14 different manufacturers
Budget Planning: Design with devices from enterprise to consumer grade


🌐 Browser Compatibility
NetScope works best on modern browsers:

✅ Chrome/Edge 90+
✅ Firefox 88+
✅ Safari 14+
✅ Opera 76+

Recommended: Chrome or Edge for best performance
