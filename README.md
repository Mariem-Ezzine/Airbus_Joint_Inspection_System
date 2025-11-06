# 🛠️ Airbus Joint Inspection System

### 🔍 Overview
This project was developed at **SAMM Test & Automation** as part of my Engineering Thesis at **ENSIT (Ecole Nationale Supérieure d’Ingénieurs de Tunis)**.  
It focuses on **real-time visual inspection of aircraft joints for Airbus**, using **computer vision** and **industrial automation** technologies.

The goal was to design an open, flexible, and maintainable system to replace a closed and expensive Cognex camera, while maintaining industrial-grade precision.

---

### ⚙️ System Description

The system performs **automatic inspection** of Airbus joint parts to detect:

- 🔴 **Holes** (using contour and circular detection)
- 🟢 **Chamfers** (via angle analysis)
- 🔵 **Curvatures** (based on contour geometry)
- 🟡 **OCR text** (using PaddleOCR for low-contrast green-on-blue text)

It integrates:

| Component | Technology |
|------------|-------------|
| Computer Vision | Python, OpenCV |
| OCR | PaddleOCR |
| Database | MySQL |
| GUI | Tkinter |
| Communication | TCP/IP with Festo CPX-E PLC |
| Hardware | FLIR industrial camera, IP Webcam |

---

### 🧩 System Architecture

```mermaid
graph TD
A[Camera (FLIR/IP)] --> B[Python OpenCV Pipeline]
B --> C[Feature Extraction: Holes, Chamfers, Curves]
B --> D[Text Recognition (PaddleOCR)]
C --> E[MySQL Database]
D --> E
E --> F[Festo PLC via TCP/IP]
B --> G[Tkinter GUI]

🖥️ Graphical Interface
Main GUI	Detection Results

	
🧠 Key Achievements

✅ Real-time image processing with OpenCV
✅ OCR of low-contrast alphanumeric codes
✅ Integration with Festo PLC (TCP/IP) for industrial communication
✅ MySQL traceability of inspections
✅ Professional Tkinter GUI for operator interaction

📊 Industrial Context

Company: SAMM Test & Automation

Client: Airbus (Safran subcontractor)

Project Type: Automated visual inspection for aerospace parts

Environment: Python 3.8, MySQL, Codesys, FLIR camera

🧰 Technologies Used

Python · OpenCV · PaddleOCR · MySQL · Tkinter · TCP/IP · PySpin · CODESYS · Festo PLC

📄 Project Origin

This work was conducted as part of my final-year engineering project (2025), supervised by
Mr. Karim Aouadi (SAMM Test & Automation) and Mr. Faouzi Benzarti (ENSIT).

The detailed technical report and source code remain private due to industrial confidentiality,
but a summary can be provided upon request.

👩‍💻 Author

Mariem Ezzine
Electrical Engineer — Computer Vision & Embedded Systems
📧 mariemezzine8@gmail.com

🔗 LinkedIn
