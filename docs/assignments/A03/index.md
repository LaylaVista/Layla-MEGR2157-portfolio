# A3 – Parametric and FEA

## Objective

The objective of this assignment is to design a bar given the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.., length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.

## Analyze

The max deflection of the bar is given as 0.009 in, the force must be between 300-500 lb, the cross-sectional area must be circular, and the material must be made of aluminum with a modulus of elasticity between (8.5-11.5) * 10^6 psi.

## Part 1 - Decide

For my material, I decided to use 6061 alloy in SolidWorks, which has a modulus of elasticity of 10.0*10^6 psi. I chose this material because it is the most common type of aluminum alloy. I decided to make the load 400 lbs because it's a nice even number, right in between 300 and 500 lbs. Then I chose the circular cross-section to have a diameter of 1 inch to keep calculations as simple as possible. I inserted all of these values into SolidWorks global variables, and I found the length using the direct tension elongation equation in the Machinery’s Handbook: L = (Defl * E * A) / F

<img width="795" height="261" alt="Screenshot 2026-09-07 180618" src="https://github.com/user-attachments/assets/1b0b0653-1492-47a3-95f7-e0dc9c3b4e39" />

## Part 2 - Conduct FEA

Once I set my global parameters, I modeled the design and ran a study, which led to the following results:

<img width="1591" height="812" alt="Screenshot 2026-09-09 085930" src="https://github.com/user-attachments/assets/feb8deea-6e65-4fc2-848a-2a1da617631a" />

The max deflection came out to be 0.009031 in.

<img width="1586" height="787" alt="Screenshot 2026-09-09 090810" src="https://github.com/user-attachments/assets/35832804-fc3d-4b87-8ce0-cb57708b2d4e" />

The maximum internal stress came out to be 551.5 psi.

<img width="947" height="663" alt="Screenshot 2026-09-09 102916" src="https://github.com/user-attachments/assets/05e5a70e-8a88-4def-8d64-99937404fa40" />

The yield strength of aluminum was given as 40 ksi, or 40,000 psi. I then calculated the safety factor using the internal stress obtained through the simulation. The safety factor came out to be 72.53.

## Part 3 - Design Reflection

<img width="1198" height="550" alt="Screenshot 2026-09-09 102925" src="https://github.com/user-attachments/assets/22528a45-f164-4597-85fd-bdbfc71e023a" />

The percentage error between the given deflection and the simulation-calculated value was 0.344%. The given and the simulation-calculated deflections were very similar. I believe this is because the geometry of the bar is very simple and uniform, with no major features(e.g., holes, fillets). I believe the hand-calculated value using the equation L = (Defl * E * A) / F is more trustworthy because it provides exact solutions for pure axial loading on a constant cross-section, whereas the FEA simulation provides a numerical approximation.

<img width="952" height="662" alt="Screenshot 2026-09-09 102931" src="https://github.com/user-attachments/assets/5f854b60-77a9-4f47-bd07-245ed3b03c09" />

I added an imaginary pinhole near the base of my bar with a diameter of 0.5 in. to see how it would affect the safety factor. I found the value of the stress concentration factor (Kt) for a hole in a flat bar in tension (Machinery's Handbook). The new calculated safety factor turned out to be 12.97, which is significantly lower than the previous safety factor. This is because when a pinhole is added to a bar, the internal stress greatly increases. 

## Part 4 - Lessons learned

 - I learned how to use FEA simulation to find numerical approximations for internal stress and deflection of a bar under a tensile load
 - I learned how adding holes in a beam affects internal stress

I spent approximately 5 hours on this assignment, with no major errors.

SolidWorks Links:

SVA6 PART.SLDPRT 
