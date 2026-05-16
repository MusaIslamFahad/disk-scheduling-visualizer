<div align="center">
 
# 💽 Disk Scheduling Visualizer

An interactive Python GUI to animate and compare disk scheduling algorithms- FCFS, SSTF, SCAN, C-SCAN, LOOK, and C-LOOK with real-time seek plots and PDF report export.
 
<p align="center">

<img src="https://img.shields.io/badge/Python-3.7+-111827?style=for-the-badge&logo=python&logoColor=FFD43B" />
<img src="https://img.shields.io/badge/GUI-Tkinter-111827?style=for-the-badge&logo=python&logoColor=4FC08D" />
<img src="https://img.shields.io/badge/License-MIT-111827?style=for-the-badge&logo=opensourceinitiative&logoColor=white" />
<img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS-111827?style=for-the-badge&logo=windows&logoColor=00A4EF" />

</p>

</div>

---
 
## 📖 Overview
 
**Disk Scheduling Visualizer** is a desktop application built for students and educators studying Operating Systems. It brings disk scheduling algorithms to life with animated head movement plots, instant seek-time results, side-by-side algorithm comparisons, and exportable PDF reports - all through a clean tkinter GUI.
 
---
 
## ✨ Features
 
- 🎬 **Live Animation**: Watch the disk head sweep across tracks in real time
- 📊 **Algorithm Comparison**: Run multiple algorithms simultaneously and compare seek times via bar chart
- 🏆 **Winner Highlight**: Automatically highlights the most efficient algorithm in green
- 📄 **PDF Report Export**: Save your simulation inputs, results, and sequence to a PDF
- 🔊 **Audio Narration**: Text-to-speech support via `pyttsx3` and `gTTS`
- 🎛️ **Configurable Parameters**: Set head position, direction, cylinder range, and request queue freely
---
 
## 🧮 Supported Algorithms
 
| Algorithm | Description |
|-----------|-------------|
| **FCFS** | First-Come, First-Served - serves requests in arrival order |
| **SSTF** | Shortest Seek Time First - always picks the nearest request |
| **SCAN** | Elevator algorithm - sweeps in one direction, then reverses |
| **C-SCAN** | Circular SCAN - sweeps one way, jumps back to the start |
| **LOOK** | Like SCAN but only goes as far as the last request |
| **C-LOOK** | Circular LOOK - jumps back to the lowest request, not cylinder 0 |
 
---

## ⚙️ Requirements
 
- Python 3.7+
- `tkinter` _(bundled with most Python installations)_
- `matplotlib`
- `numpy`
- `pyttsx3`
- `gTTS`
- `fpdf`
- `Pillow`
---
 
## 🚀 Getting Started
 
**1. Clone the repository**
```bash
git clone https://github.com/MusaIslamFahad/disk-scheduling-visualizer.git
cd disk-scheduling-visualizer
```
 
**2. Install dependencies**
```bash
pip install matplotlib numpy pyttsx3 gTTS fpdf Pillow
```
 
**3. Run the application**
```bash
python OS_PROJECT.py
```
 
---
 
## 🕹️ How to Use
 
### Practice Tab
1. Enter a comma-separated list of disk request points (e.g., `98, 183, 37, 122, 14`)
2. Set the **Initial Head Position** (e.g., `53`)
3. Choose a **Direction** (`LEFT` or `RIGHT`) for directional algorithms
4. Select an algorithm from the dropdown
5. Click **RUN** to watch the animation
6. Click **SAVE** to export a PDF report
### Comparison Tab
1. Use the same inputs as above
2. Check all the algorithms you want to compare
3. Click **RUN COMPARISON** to see a bar chart — the green bar is the winner
---
 
## 📁 Sample Simulation
 
| Parameter | Value |
|-----------|-------|
| Request Queue | `98, 183, 37, 122, 14, 124, 65, 67` |
| Head Start | `53` |
| Direction | `RIGHT` |
| Max Cylinder | `200` |
 
**Expected outcome:** SSTF typically produces the lowest total seek time; FCFS the highest. SCAN shows the classic elevator sweep pattern.
 
---
 
## 📂 Project Structure
 
```
disk-scheduling-visualizer/
│
├── -VISUALISATION-OF-DISK-SCHEDULING-ALGORITHM-USING-GUI-PYTHON-main/
│   └── OS_PROJECT.py       # Main application entry point
│
└── README.md
```
 
---
 
## 🤝 Contributing
 
Contributions are welcome! To contribute:
 
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request
---
 
## 📜 License
 
This project is licensed under the [MIT License](LICENSE).
 
---
 
## 👨‍💻 Author
 
**Musa Islam Fahad**
- GitHub: [@MusaIslamFahad](https://github.com/MusaIslamFahad)
---
 
> ⭐ If you found this project helpful, please give it a star. It motivates further development!
