# ✈️ Aerodynamic Analysis of Cessna 172 Wing: Navier-Stokes vs Euler Methods 🛩️

This project compares the aerodynamic performance of a flat plate airfoil using two fundamentally different flow models:

- **Euler-based analytical solution**  
  (ideal, inviscid, irrotational)

- **Navier-Stokes-based simulation data**  
  (realistic, viscous, includes boundary layer and possible stall)

The comparison is made by plotting the **lift coefficient (CL)** and **drag coefficient (CD)** as functions of the angle of attack (α), using both the analytical formula and polar data files from simulation.

---

## 📐 Theoretical Background

### ✅ Euler-Based CL Formula

In the case of **ideal, incompressible, inviscid (Eulerian) flow**, the lift coefficient for a thin airfoil is given by:

\[
C_L = 2\pi \alpha
\]

Where:
- \( \alpha \) is the angle of attack (in **radians**),
- The airfoil is assumed to be **infinitely thin**,
- **No flow separation** or **stall** is considered.

This formula is derived from **thin airfoil theory**, which is based on the **Euler equations** and potential flow assumptions.  
The **Kutta condition** is applied at the trailing edge to ensure smooth flow detachment.

> 🔎 For small angles of attack (e.g., \( \alpha < 10^\circ \)), this approximation is highly accurate even for cambered or rounded airfoils.

---

### ⚠️ Note on Navier-Stokes Models

Real viscous flow (modeled by the **Navier-Stokes equations**) includes:
- Boundary layer formation
- Flow separation
- Skin friction drag
- Stall behavior at high angles

Therefore, the actual lift and drag curves deviate from the ideal Euler predictions as α increases, especially beyond stall.

---

## 📚 References

- Anderson, J. D. *Fundamentals of Aerodynamics*, McGraw-Hill  
- Abbott & Von Doenhoff, *Theory of Wing Sections*, Dover Publications  

---

## 🧠 Notes

While the **Euler-based solution** tends to overestimate lift at high angles of attack due to the lack of stall modeling, it provides excellent insight into the **fundamental aerodynamic behavior** of airfoils under ideal conditions.  
The **Navier-Stokes data**, by contrast, captures **real-world phenomena** like boundary layer behavior and flow separation with much higher fidelity.

---

## 📬 Author

**Helin Hilda Uluğtürken**  
Saint Michel High School  
Aspiring Aerospace & AI Engineer
