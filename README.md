# ✈️ Aerodynamic Analysis of Cessna 172 Wing: Navier-Stokes vs Euler Methods 🛩️

Welcome to this aerodynamic analysis project conducted during my internship at Sorbonne University, focusing on the Cessna 172 aircraft wing.

---

## Project Overview

This project compares two fundamental computational fluid dynamics (CFD) approaches — **Navier-Stokes** and **Euler** methods — to analyze the lift (CL) and drag (CD) coefficients of the Cessna 172 wing using polar data from XFOIL simulations.

- **Navier-Stokes data** were obtained using XFOIL with viscosity and Mach number effects included, providing realistic drag coefficients.
- **Euler method** was implemented by calculating CL and estimating CD with a simplified assumption (constant minimal drag) since Euler equations neglect viscosity.

---

## Why is the Drag Coefficient (CD) zero in Euler calculations?

Since the Euler equations ignore viscous effects, the drag computed by the Euler method is typically underestimated or near zero. This is because:

- **Viscosity is the main contributor to drag (skin friction and pressure drag).**
- Without including viscosity in the model, Euler-based drag calculations cannot capture these real aerodynamic losses.
- In contrast, the Navier-Stokes method incorporates viscosity, resulting in more accurate drag coefficient values.

---

## Data and Methods

- Wing geometry and polar data were generated using **XFOIL**, a well-known airfoil analysis tool.
- Flight conditions and aircraft specifications for the **Cessna 172** were taken from publicly available general characteristic data, including altitude-dependent air density and cruise speed.
- The project includes Python scripts that calculate lift and drag forces based on both methods, with detailed graphs comparing CL and CD across angles of attack.

---

## How to use this repository

- Check the `scripts/` folder for source codes.
- Input files include Navier-Stokes polar data (`naca2412polar_navier.txt`) and Euler polar data (`polar_EULER2412.txt`).
- Run the scripts to generate comparative plots of lift and drag coefficients.
- Explore modifications or extend the models with more sophisticated CFD tools or real flight data.

---

## Acknowledgments

Thanks to Sorbonne University for the opportunity to gain practical experience in aerospace aerodynamics through this internship.

---

Feel free to contribute, ask questions, or suggest improvements! 😊

