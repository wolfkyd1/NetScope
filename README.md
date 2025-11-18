# 📡 NetScope - Professional RF Network Design Tool

A powerful, browser-based WiFi network planning and RF propagation modeling tool for designing enterprise wireless networks. Plan your WiFi coverage with real-time heatmaps, wall attenuation modeling, and comprehensive AP placement analysis.

![NetScope Interface](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

---

## ✨ Features

### 🗺️ **Floor Plan Integration**
- Upload floor plans as images (PNG, JPG) or PDF files
- Automatic PDF-to-image conversion
- Precise scale calibration tool for accurate measurements
- Pan and zoom controls for detailed planning

### 📶 **Access Point Management**
- **Extensive device library** with 40+ pre-configured APs from:
  - **Aruba** (AP-325, AP-515, AP-555, AP-635, AP-655, AP-505H, AP-387)
  - **Grandstream** (GWN7630LR, GWN7660, GWN7664, GWN7605, GWN7610, GWN7602, GWN7000/7001 Routers)
  - **MikroTik** (cAP ac, wAP ac, cAP XL ac, Audience, BaseBox 5, SXTsq 5 ac, hAP series)
  - **TP-Link** (EAP225, EAP245, EAP620 HD, EAP650, EAP655, EAP660 HD, Archer series)
- Drag-and-drop AP placement
- Real-time signal coverage visualization
- Configurable AP settings:
  - Transmit power (2.4 GHz & 5 GHz)
  - Channel assignment
  - Antenna type (omnidirectional/directional)
  - Antenna orientation
  - Mounting height

### 🧱 **Wall & Obstacle Modeling**
- Draw walls with click-to-place interface
- Smart wall snapping for room creation
- Material-based attenuation modeling:
  - Glass (3 dB)
  - Wood (5 dB)
  - Drywall (8 dB)
  - Concrete (12 dB)
  - Brick (15 dB)
  - Metal/Elevator Shafts (20 dB)
- Automatic room detection
- Editable wall properties

### 🔥 **RF Propagation & Heatmaps**
- Real-time signal strength heatmaps
- Free Space Path Loss (FSPL) calculations
- Wall attenuation modeling
- Multiple resolution settings (Low/Medium/High)
- Adjustable heatmap opacity
- Coverage circles visualization
- Signal strength at any point (click-to-measure)

### 👥 **Client Simulation**
- Simulate 10-200 WiFi clients
- Automatic AP association
- Client density heatmaps
- Real-time speed estimates based on RSSI:
  - WiFi link speed calculation
  - Download/upload bottleneck analysis
  - Per-client signal strength visualization

### 📊 **Analysis Tools**
- **Auto-Channel Planning**: Automatically assigns non-overlapping channels
- **Interference Detection**: Visualize co-channel and adjacent-channel interference
- **Coverage Statistics**: Real-time coverage percentage calculations
- **Room Analysis**: Automatic room detection with area calculations
- **Measurement Tool**: Click-to-measure distances in feet
- **Signal Analysis**: Point-and-click signal strength analysis

### 📤 **Export Capabilities**
- **PDF Reports** including:
  - Project summary
  - AP configuration details
  - Coverage heatmap visualization
  - Room listings
- **PNG Heatmap Export**: High-resolution coverage maps
- **JSON Project Files**: Save and load complete projects

---

## 🚀 Getting Started

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/netscope.git
   cd netscope
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
   - Select your AP model from the device library
   - Click on the floor plan to place the AP

4. **Draw Walls** 🧱
   - Click the "Wall" tool
   - Click to place points along walls
   - Double-click or press ESC to finish
   - Select wall material type when prompted

5. **View Coverage** 🔥
   - Coverage heatmap updates automatically
   - Toggle heatmap visibility in bottom-left controls
   - Adjust opacity and resolution as needed

6. **Simulate Clients** 👥
   - Set client count in the right panel (10-200)
   - Click "Simulate Clients"
   - View client connections and density

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

### Signal Quality Thresholds
- **Excellent**: > -50 dBm (1.2 Gbps)
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
└── examples/           # Example projects
    ├── office.json
    ├── warehouse.json
    └── retail.json
```

---

## 🎯 Use Cases

- **Enterprise WiFi Planning**: Design optimal AP placement for offices and campuses
- **Warehouse Networks**: Plan coverage for large industrial spaces
- **Retail Deployments**: Ensure coverage in customer areas
- **Venue WiFi**: Design networks for stadiums, conference centers, hotels
- **Education**: Network planning for schools and universities
- **Healthcare**: RF planning for hospitals with strict coverage requirements
- **IoT Deployments**: Plan coverage for IoT device connectivity

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'Add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Feature Requests & Bug Reports

Please use GitHub Issues to report bugs or request features.

**When reporting bugs, please include:**
- Browser version
- Steps to reproduce
- Expected vs actual behavior
- Screenshots if applicable

---

## 📝 Roadmap

- [ ] 6 GHz (WiFi 6E) support
- [ ] 3D visualization mode
- [ ] Multi-floor planning
- [ ] Outdoor propagation models
- [ ] Bill of Materials (BOM) export
- [ ] Integration with vendor APIs
- [ ] Real-time collaboration
- [ ] Mobile app version
- [ ] Advanced interference analysis
- [ ] Cost estimation tools

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- Device specifications sourced from manufacturer datasheets
- RF propagation models based on IEEE 802.11 standards
- Inspired by professional tools like Ekahau and iBwave

---

## 📞 Support

- **Documentation**: [Wiki](https://github.com/yourusername/netscope/wiki)
- **Issues**: [GitHub Issues](https://github.com/yourusername/netscope/issues)
- **Discussions**: [GitHub Discussions](https://github.com/yourusername/netscope/discussions)

---

## 🌟 Star History

If you find NetScope useful, please consider giving it a star! ⭐

---

<div align="center">

**Made with ❤️ by the NetScope Team**

[Report Bug](https://github.com/yourusername/netscope/issues) · [Request Feature](https://github.com/yourusername/netscope/issues) · [Documentation](https://github.com/yourusername/netscope/wiki)

</div>
