# pca-variance-interactive-visualiser
## 🔦 The Shadow Machine

**The Shadow Machine** is an interactive, web-based educational instrument designed to intuitively visualize the core concept behind **Principal Component Analysis (PCA)**. 

Instead of focusing on finding a line of best fit by minimizing vertical error (Linear Regression), this tool asks a different question: *In which direction is the data most spread out?* By rotating a beam and watching the "shadows" (projections) of the data points, users manually discover the axis of maximum variance.

---

## ✨ Features

* **Interactive Data Cloud:** Click empty space to add points, drag them to reshape the cloud, or double-click to remove them.
* **Rotatable Beam:** Drag the gold handle or use the slider to sweep the beam 180 degrees to test different projection angles.
* **Real-Time Spread Calculation:** Watch the variance calculate instantly as you rotate the beam or move data points.
* **Live Progress Tracking:** A dynamic percentage bar and live feedback text show exactly how close you are to finding the optimal angle.
* **Interactive Curve Plotting:** A secondary graph automatically plots the variance across all angles, visually proving that the "gold peak" is the objective mathematical answer.
* **Zero Dependencies:** Built entirely with vanilla web technologies in a single file.

---

## 🧮 The Math: Maximum Variance

This tool demonstrates the first step of Principal Component Analysis (PCA): finding the first principal component. It calculates the mean of the data points, projects each point onto the beam's directional vector, and calculates the variance of those projections.

The math running under the hood to calculate the spread (variance) is:

$$ \text{Variance} = \frac{1}{N} \sum_{i=1}^{N} ((x_i - \bar{x})\cos(\theta) + (y_i - \bar{y})\sin(\theta))^2 $$

Where $(x_i, y_i)$ are the data points, $(\bar{x}, \bar{y})$ is the centroid (mean), and $\theta$ is the angle of the beam. 

---
