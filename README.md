# ✈️ Aerodynamic Analysis of Cessna 172 Wing: Navier-Stokes vs Euler Methods 🛩️

This project compares the aerodynamic performance of a flat plate airfoil using two fundamentally different flow models:

- **Euler-based analytical solution** (ideal, inviscid, irrotational)
- **Navier-Stokes-based simulation data** (realistic, viscous, possibly including stall)

The comparison is made by plotting **lift coefficient (CL)** and **drag coefficient (CD)** as functions of the angle of attack (α), using both analytical formulas and polar data files.

---

## 📐 Theoretical Background

### ✅ Euler-Based CL Formula

In the case of **ideal, incompressible, inviscid (Eulerian) flow**, the lift coefficient for a thin airfoil is given by:

\[
\boxed{C_L = 2\pi \cdot \alpha}
\]

Where:
- \( \alpha \) is the angle of attack (in **radians**)
- The airfoil is assumed to be **infinitely thin**
- No flow separation or stall is considered

This formula is derived from **thin airfoil theory**, which itself is based on the **Euler equations** and potential flow assumptions. The trailing edge behavior is resolved by enforcing the **Kutta condition**.

> 🔎 At small angles (e.g., \( \alpha < 10^\circ \)), this approximation is highly accurate even for cambered or rounded airfoils.

### ⚠️ Note on Navier-Stokes Models

Real viscous flow (modeled by Navier-Stokes equations) includes boundary layer effects, flow separation, and stall. Therefore, the actual lift curve deviates from the Euler solution at higher angles of attack.

---

## 📚 References
Anderson, J. D. Fundamentals of Aerodynamics, McGraw-Hill

Abbott & Von Doenhoff, Theory of Wing Sections, Dover Publications

NASA Glenn Research Center: Airfoil Theory

🧠 Notes
While the Euler solution overestimates lift at high angles of attack due to the lack of stall modeling, it provides excellent insight into the fundamental aerodynamic behavior of airfoils in ideal conditions. The Navier-Stokes data captures real-world behavior including flow separation, skin friction, and stall.

📬 Author
Helin Hilda Uluğtürken
Saint Michel High School



