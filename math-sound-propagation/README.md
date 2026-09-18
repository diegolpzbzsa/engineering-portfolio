\# Mathematical Modeling of Sound Propagation in Variable-Geometry Trumpets



\## Overview



This project was my IB Mathematics Internal Assessment. I investigated how the geometry of a trumpet affects the propagation of sound by modeling acoustic pressure using differential equations.



The main goal was to connect a physical system with a mathematical model and then study how changing one geometric parameter, the radius of the trumpet, changes the predicted behavior of the wave.



\## Research Goal



How does the geometry of a trumpet affect the propagation of sound inside it?



I compared three idealized geometries:



\- constant radius

\- linearly increasing radius

\- exponentially increasing radius



\## Developing the Model



I began from the acoustic wave equation and then used the Webster horn equation to incorporate the changing cross-sectional area of the trumpet.



After representing the area as



A(x) = πr(x)²



and separating the pressure into spatial and temporal components,



p(x,t) = Φ(x) sin(ωt),



I obtained an ordinary differential equation for the spatial component of the pressure:



d²Φ/dx² + (2/r)(dr/dx)(dΦ/dx) + (ω²/c²)Φ = 0



This equation allowed the geometry of each trumpet to enter the model directly through the radius function r(x).



\## Numerical Method



For the variable-radius cases, I converted the second-order differential equation into a system of first-order equations and solved it numerically using Euler's method.



I implemented the numerical calculations in Excel using small spatial steps to estimate the evolution of both Φ(x) and its derivative.



This allowed me to compare the predicted pressure behavior for different trumpet geometries even when the differential equation was difficult to solve analytically.



\## Constant-Radius Model



For a cylindrical tube,



dr/dx = 0,



so the equation reduces to a simple harmonic oscillator.



The resulting model predicts a sinusoidal wave with constant amplitude, and the corresponding phase diagram forms a closed ellipse.



<!-- Add constant-radius result image here -->



\## Linear-Radius Model



I measured the profile of a trumpet with approximately linear expansion and fitted the radius as a function of position.



The numerical solution predicted an increasing wave amplitude as the radius increased. In the idealized model, the maximum amplitude grows approximately linearly with position.



<!-- Add linear-profile image here -->



<!-- Add linear numerical-result image here -->



\## Exponential-Radius Model



I repeated the process for a trumpet with an approximately exponential profile.



The model predicted much stronger amplitude growth, particularly as the wave entered the bell. The corresponding phase diagram expanded rapidly, reflecting the exponential behavior of the idealized solution.



<!-- Add exponential result image here -->



\## Comparison



The three models produced clearly different behaviors:



| Geometry | Predicted behavior |

| --- | --- |

| Constant radius | Approximately constant amplitude |

| Linear radius | Approximately linear amplitude growth |

| Exponential radius | Strong exponential amplitude growth |



Within the assumptions of the model, this showed how the geometry of the instrument enters directly into the differential equation and changes the predicted propagation of the acoustic wave.



\## Limitations



The model is intentionally idealized.



It does not fully account for effects such as energy dissipation in air, acoustic losses, sound escaping from the instrument, or reflections and interference at the bell.



These effects become especially important in the exponential model, where the mathematical solution grows much faster than would be physically realistic.



A more advanced model could include damping and more realistic boundary conditions.



\## What I Learned



This project helped me understand differential equations as more than an abstract mathematical topic.



I started with a physical problem, identified the variables that mattered, built a differential equation that connected them, solved the equation numerically, and then interpreted what the mathematical result meant physically.



It also showed me the importance of understanding the assumptions behind a model. A mathematical solution can be internally consistent while still requiring limits before it can represent a real physical system accurately.



\[← Back to Engineering Portfolio](../)

