# A3 – Parametric and FEA

## Objective

The objective of this assignment is to design a bar given the material, maximum deflection, and load. Determine the bar’s minimum geometry (ie.., length, diameter, and weight) through parametric design while under direct tension. Then verify the geometry through finite element analysis.

## Analyze

The max deflection of the bar is given as 0.009 in, the force must be between 300-500 lb, the cross-sectional area must be circular, and the material must be made of aluminum with a modulus of elasticity between (8.5-11.5)*10^6 psi.

## Decide

For my material, I decided to use 6061 alloy in SolidWorks, which has a modulus of elasticity of 10.0*10^6 psi. I chose this material because it is the most common type of aluminum alloy. I decided to make the load 400 lbs because it's a nice even number, right in between 300 and 500 lbs. Then I chose the circular cross-section to have a diameter of 1 inch to keep calculations as simple as possible. I inserted all of these values into SolidWorks global variables, and I found the length using the direct tension elongation equation in the Machinery’s Handbook: L = Defl**E**A/F



## Communicate

