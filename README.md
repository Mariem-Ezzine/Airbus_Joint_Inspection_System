# Airbus Joint Inspection System

A real-time computer vision and automation system for inspecting Airbus aircraft joints.  
Developed at **SAMM Test & Automation** as part of an engineering thesis at **ENSIT (Ecole Nationale Supérieure d’Ingénieurs de Tunis)**.

This project replaces an expensive industrial Cognex camera with an **open Python-based solution** integrating:
- **OpenCV** for geometric defect detection (holes, chamfers, curvatures)
- **PaddleOCR** for text recognition (green on blue surfaces)
- **MySQL** for traceability and report storage
- **TCP/IP communication** with a **Festo CPX-E-CEC-M1-PN PLC**
- **Tkinter GUI** for real-time visualization and control
