# PID Controller Simulation with Streamlit 🎮

An interactive dashboard for exploring PID control on various second-order systems, built with Streamlit and Bokeh.

![Python](https://img.shields.io/badge/python-v3.11-blue.svg)
![Streamlit](https://img.shields.io/badge/streamlit-v1.29-red.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)

## 🌟 Features

- Interactive PID controller parameter adjustment
- Multiple predefined system types:
  - Pure Oscillator (Undamped)
  - Underdamped Mechanical System
  - Chemical Reactor
  - Fast Servo Motor
  - Critically Damped Load
  - Custom System
- Real-time visualization of:
  - Process Variable vs Setpoint
  - Control Signal
  - Error
- System performance metrics
- Educational explanations of system dynamics

## 🚀 Getting Started

### Prerequisites

- Python 3.11 (recommended)
- Git (for cloning the repository)

### Installation

1. Clone the repository:
```bash
git clone git@github.com:Haavi97/PIDController.git
cd PIDController
```

2. Create and activate a virtual environment:
```bash
# On Windows
python -m venv venv
.\venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

### Running the Application

1. Start the Streamlit server:
```bash
streamlit run pid_controller.py
```

2. Open your web browser and navigate to:
```
http://localhost:8501
```

## 📦 Dependencies

Create a `requirements.txt` file with the following contents:

```
streamlit>=1.29.0
numpy>=1.24.0
bokeh>=3.0.0
```

## 🌐 Live Demo

Check out the live demo on Streamlit Cloud:
[PID Controller Simulation Demo](https://pid-controller-simulation.streamlit.app)

## 🚀 Deployment

### Deploying to Streamlit Cloud

1. Create a Streamlit Cloud account:
   - Go to [share.streamlit.io](https://share.streamlit.io)
   - Sign in with GitHub

2. Prepare your repository:
   - Ensure your code is in a public GitHub repository
   - Verify requirements.txt is present and up-to-date
   - Make sure streamlit run pid_controller.py works locally

3. Deploy on Streamlit Cloud:
   - Click "New app" on Streamlit Cloud
   - Select your repository, branch, and main file (pid_simulator.py)
   - Click "Deploy"

Your app will be available at: `https://<your-app-name>.streamlit.app`

### Advanced Deployment Options

1. Custom domain setup:
   - Go to your app settings in Streamlit Cloud
   - Navigate to "Custom domain"
   - Follow the DNS configuration instructions

2. Environment variables: in the dropdown menu select the 3.11 Python version

## 🎮 Usage

1. Select a system type from the dropdown menu
2. Adjust PID controller parameters:
   - Kp (Proportional gain)
   - Ki (Integral gain)
   - Kd (Derivative gain)
3. Set your desired setpoint
4. Observe the system's response in real-time
5. Monitor performance metrics in the sidebar

## 🔍 System Types Explained

### Pure Oscillator (Undamped)
- No natural damping
- Continuous oscillation without energy loss
- Ideal for understanding the need for control

### Underdamped Mechanical System
- Similar to car suspension
- Natural oscillations that decay over time
- Good for demonstrating derivative control

### Chemical Reactor
- Slower system dynamics
- Thermal lag characteristics
- Demonstrates the need for integral control

### Fast Servo Motor
- Quick response system
- High natural frequency
- Shows the importance of derivative damping

### Critically Damped Load
- Optimal natural damping
- No oscillation
- Fastest non-oscillatory response

### Custom System
- Fully adjustable parameters
- Experimental platform
- Great for learning system dynamics

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the `LICENSE` file for details.

## ✨ Acknowledgments

- Control Systems Theory
- Streamlit Community
- Bokeh Visualization Library