# Epitrochoidal-Surface

### **What is an Epitrochoidal Surface?**  
An **epitrochoidal surface** is a 3D surface generated by tracing a point attached to a circle as it rolls around another fixed circle. It is a generalization of an **epitrochoid**, which is a 2D curve. These surfaces are particularly useful in **mechanical engineering**, especially in **rotary engines** like the Wankel engine.  

### **Equation Used in Your Code**  
The equation you used to generate the epitrochoidal surface is:

\[
\begin{cases}
x = 2R \cos(v)^2 \cos(u) \\
y = 2R \cos(v)^2 \sin(u) \\
z = R \sin(2v)
\end{cases}
\]

where  
- \( u \) and \( v \) are parametric variables that range from \( -\pi \) to \( \pi \).  
- \( R \) is a function that defines the varying radius of the surface:  

  \[
  R = a (1 + m \cos(u))
  \]

  with constants \( a \) and \( m \), which affect the shape of the surface.

---

### **Breaking Down the Equation**
1. **Radial Function \( R \)**
   - The function \( R = a (1 + m \cos(u)) \) controls the size of the radius at different values of \( u \).
   - When \( m = -1 \), the surface exhibits periodic shrinking and expansion.

2. **X and Y Coordinates**
   - The **\( x \) and \( y \) equations** define a circular motion that is scaled by \( 2R \cos^2(v) \).
   - This means that as \( v \) varies, the points on the surface will move in a way that resembles **nested, deformed circular layers**.

3. **Z Coordinate**
   - The **\( z \)-coordinate** follows a **sinusoidal wave**: \( z = R \sin(2v) \).
   - This gives the surface its characteristic **undulating, wave-like appearance**.

---

### **Why This Surface Looks Like the Image?**
- The **wireframe-like appearance** is due to using a **grid of points** from \( u \) and \( v \) values.
- The **color gradient** is applied using the hue from the **HSV color space**, inspired by the colors in the reference image.
- The **3D twisting effect** comes from how **\( R \)** changes over \( u \), modifying how the shape extends outward.
