✈️ Aerodynamic Analysis of Cessna 172 Wing: Navier-Stokes vs Euler Methods 🛩️
This project compares the aerodynamic lift and drag coefficients of the Cessna 172 wing using two fundamental fluid dynamics approaches: Navier-Stokes and Euler equations.

🚀 Overview
Navier-Stokes data is generated using XFOIL, capturing viscous effects like skin friction and turbulence, resulting in realistic drag coefficient (CD) values. 🌀

Euler method models inviscid flow, predicting lift coefficient (CL) well but neglecting viscous drag, leading to underestimated or zero drag values. ❌💨

📊 What’s inside
Reading and processing polar data from XFOIL for Navier-Stokes solutions. 📂

Calculating Euler-based lift and drag coefficients using pressure difference and flight conditions. ⚙️

Comparison graphs of CL and CD vs. angle of attack. 📈

Altitude-dependent air density calculations to simulate realistic flight conditions. 🌤️

❓ Why does CD differ between Euler and Navier-Stokes?
Euler equations assume no viscosity, so drag related to friction (viscous drag) is missing in calculations. This results in drag coefficients near zero, unlike Navier-Stokes results which include these effects. 🧪🛑

🛠️ Technologies & Tools
Python 3 🐍

NumPy & Matplotlib 📊

XFOIL (for polar data generation) 💻

💻 How to run
Clone the repository 📥

Place the polar data files (naca2412polar_navier.txt for Navier-Stokes, polar_euler2412.txt for Euler) in the same folder. 📂

Run the main Python script:

bash
Copier
python aerodynamic_analysis.py
👨‍🎓 About Me
This project was developed during my aerodynamics internship at Sorbonne University. It gave me hands-on experience with CFD methods and practical understanding of fluid flow effects on aircraft wings. ✈️🔥
