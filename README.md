# Makinaut

**Plug. Code. Control.**

Makinaut is an intuitive Python-based framework that lets you control motors, sensors, and other hardware from a web interface — without needing to write frontend code or complex logic. Whether you're a beginner with a breadboard or an expert automating a lab, Makinaut gets you up and running fast.

---

## 🎯 Vision
Makinaut empowers makers, students, and developers to rapidly build hardware control systems with minimal setup, no prior software experience, and a fun, intuitive experience. Whether you're a beginner with a breadboard or an expert with a robotic system, Makinaut helps you plug, code, and control — fast.

---

## 🚀 Features
- ✅ YAML-based plug & play hardware config
- ✅ Auto-generated control dashboard
- ✅ Support for motors, sensors, GPIO devices
- ✅ Beginner-friendly setup, advanced flexibility
- ✅ Modular device architecture
- ✅ Flask-powered local web UI

---

## 🧪 Quick Start

### 1. Clone the Repo
```bash
git clone https://github.com/YOUR_USERNAME/makinaut-core.git
cd makinaut-core
```

### 2. Set up a virtual environment (Windows example)
```bash
python -m venv venv
venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
python web/app.py
```

Go to `http://127.0.0.1:5000` in your browser to control your hardware.

---

## 🔧 Example `makinaut.yaml`
```yaml
components:
  - name: test_motor
    type: stepper_motor
    pins: [17, 18, 27, 22]  # Example GPIO pins
```

---

## 🧠 Project Structure
```
makinaut-core/
├── README.md
├── makinaut.yaml              # Main project configuration file
├── core/
│   ├── __init__.py
│   ├── engine.py              # Core logic loader
│   └── config_loader.py       # Parses makinaut.yaml
├── devices/
│   ├── stepper_motor.py       # Device plugin: stepper motor
│   └── dht22_sensor.py        # Device plugin: DHT22 sensor
├── web/
│   ├── __init__.py
│   ├── app.py                 # Web server (Flask)
│   ├── routes.py              # UI endpoints
│   └── templates/
│       └── dashboard.html     # Auto-generated UI frontend
└── requirements.txt           # Python dependencies
```

---

## 🔮 Coming Soon
- UI builder
- Live sensor charts
- Device marketplace
- Cloud deployment support
- CLI: `makinaut init`, `makinaut add`, `makinaut run`

---

## 📬 Feedback & Ideas
Makinaut is built to help people learn, build, and innovate faster.  
Have a cool idea? Found a bug? Want to contribute?  
Open an issue or get in touch!
