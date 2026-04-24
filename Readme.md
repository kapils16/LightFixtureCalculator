# Lighting Fixture Calculator (Lumen Method)

A high-precision, browser-based lighting design tool that calculates the required number of luminaires and generates an optimal grid layout using the **CIBSE Lumen Method**.

## 🚀 Features

* **Real-Time SVG Schematic:** Visualizes fixture placement, spacing ($S_x, S_y$), and border distances.
* **Lumen Method Engine:** Calculates $N$ based on target Illuminance, Luminous Flux, and Maintenance Factors.
* **Automated UF Interpolation:** Performs linear interpolation of **Utilisation Factors** based on Room Index ($RI$) and surface reflectances.
* **Uniformity Check:** Monitors the Spacing-to-Height Ratio ($S/Hm$) and warns if it exceeds $1.5$.
* **Dark Mode Interface:** Built with a modern, high-contrast engineering aesthetic.

## 📐 The Formulae

The calculator operates on the following core principles:

1.  **Number of Fixtures ($N$):**
    $$N = \frac{E \times A}{\Phi \times UF \times MF}$$
2.  **Room Index ($RI$):**
    $$RI = \frac{L \times W}{Hm \times (L + W)}$$
3.  **Mounting Height ($Hm$):**
    $$Hm = CeilingHeight - WorkplaneHeight - SuspensionLength$$

## 🛠️ Installation & Usage

This is a portable, single-file web application. No installation or dependencies are required.

1.  Download the `index.html` file (or the HTML code provided).
2.  Open the file in any modern web browser (Chrome, Firefox, Edge, Safari).
3.  Adjust the **Room Geometry** and **Luminaire** inputs in the left panel.
4.  The **Schematic Plan** and **Results** will update instantly.

## 📋 Input Parameters

| Parameter | Description | Typical Value |
| :--- | :--- | :--- |
| **Length/Width** | Physical dimensions of the room (m) | - |
| **Work Plane** | Height where task light is measured | 0.85m (Desk height) |
| **Required E** | Target illuminance in Lux (lx) | 500lx (Office) |
| **Flux ($\Phi$)** | Light output per fixture (Lumens) | 3000lm |
| **MF** | Maintenance Factor (dirt/aging) | 0.80 |

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.
