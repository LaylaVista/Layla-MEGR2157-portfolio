# A4 – Motor Mount

## Objective

Design a motor mount consisting of two features. Design both features for yield strength and for maximum deflection. The max deflection is to be 0.3mm, and the safety factor is 3.0 for both features. The mount will be made out of ABS. Sketch the final design as an isometric view, and then 3D model the design in SolidWorks using parametric modeling techniques when applicable. 

The motor dimensions are given below along with the design constraints of features 1 and 2. The force applied is given as 300N to the right. 

<img width="1038" height="318" alt="Screenshot 2026-09-12 144448" src="https://github.com/user-attachments/assets/5f64dc59-8e49-4508-aedc-b03ee6774db3" />

<img width="400" height="350" alt="Screenshot 2026-09-13 120815" src="https://github.com/user-attachments/assets/c8120a21-72b1-4683-9f27-7c05b0a6151b" />

<img width="400" height="400" alt="Screenshot 2026-09-13 122055" src="https://github.com/user-attachments/assets/108f3469-4e61-40e5-ae74-bbcff160daf9" />

## Part 1 - Feature 1

Since the maximum diameter of the motor is 28mm, I decided the length L would be 34 mm, and the width b would be 40mm, since I wanted feature 1 to be bigger than the actual motor. I then solved for the moment that feature 1 will be subjected to. 

<img width="600" height="400" alt="Screenshot 2026-09-13 123253" src="https://github.com/user-attachments/assets/e5eb7a53-8626-44dc-88a4-2b3fe0634108" />


<ins>Knowns</ins>:

δmax = max. deflection(0.3mm)

M = max. bending moment(5400Nmm)

L = length(34mm

b = width(40mm)

E = Modulus of Elasticity(2000MPa)

SF = Safety Factor(3)

Sy = Yield Strength(40MPa)


<ins>Unknowns</ins>:

Minimum value of h


I need to determine the minimum value of h using the beam bending equations from the lecture, which are given below. In the equation, I set σ<sub>max</sub> = Sy/SF, and the mass moment of inertia of a rectangle equal to bh^3/12.

<img width="500" height="400" alt="Screenshot 2026-09-13 123245" src="https://github.com/user-attachments/assets/f74b9e7a-d12a-4dfe-a3f0-ed609a292193" />

<img width="1112" height="500" alt="Screenshot 2026-09-16 081853" src="https://github.com/user-attachments/assets/adf4e814-e18f-486b-bea0-e08c30d6bbc6" />

Now I can solve these equations for h, and then plug in the known values to solve for h<sub>min</sub>.

| h due to stress | h due to deflection |
| --- | --- |
| h<sub>strength</sub> = 7.794mm | h<sub>stiffness</sub> = 16.729mm |

Since h<sub>stiffness</sub> > h<sub>strength</sub> , we set h<sub>min</sub> = h<sub>stiffness</sub> = 16.729mm. I chose the largest value for h<sub>min</sub> because the stiffness is going to fail before the strength; therefore, the height has to accommodate stiffness. 

## Part 2 - Feature 2

The total length of the motor was 74.7mm, so I decided to make the length of feature 2 75mm. The width b is the same as feature 1. I then decided on the location of the bolts. I solved for the moment the same way as I did in feature 1; however, I took the moment about the bolt that was closest to the applied force. Now, I only need to solve for thickness t.

<img width="1156" height="664" alt="Screenshot 2026-09-13 131941" src="https://github.com/user-attachments/assets/25257048-a6d0-4943-ac69-ff88030d5df2" />

Using the same equation as I did in feature 1, I solved for t:

| t due to stress | t due to deflection |
| --- | --- |
| t<sub>strength</sub> = 11.325mm | t<sub>stiffness</sub> = 23.112mm |

Since t<sub>stiffness</sub> > t<sub>strength</sub> , we set t<sub>min</sub> = t<sub>stiffness</sub> = 23.112mm.

## Part 3 - Isometric View

<img width="668" height="662" alt="Screenshot 2026-09-13 141749" src="https://github.com/user-attachments/assets/60ee34a4-784e-4bc4-bc19-5c30a5d03c1f" />


## Part 4 - CAD Model

Using the global parameters in SolidWorks, I set the height and the thickness to the calculated values.

<img width="700" height="300" alt="Screenshot 2026-09-13 142146" src="https://github.com/user-attachments/assets/2da348a7-785c-4b43-ab3d-525cdb809fc7" />

<img width="300" height="400" alt="Screenshot 2026-09-13 142131" src="https://github.com/user-attachments/assets/c8b46157-1500-428c-bf90-a1af04b9891a" />

The diameter of the innermost circle was to be 6mm, and I extrude cut through the entire mount. The diameter of the second innermost circle was 18mm, which I cut only 2mm down into the mount.

<img width="400" height="400" alt="Screenshot 2026-09-13 142315" src="https://github.com/user-attachments/assets/bbe72f48-6464-4f71-9854-4c0d068036e9" />

<img width="425" height="400" alt="Screenshot 2026-09-13 142409" src="https://github.com/user-attachments/assets/5c48d971-2d6c-4c90-8526-94c8295134cd" />

Then I made the holes for the bolts using a circular pattern to match the dimensions of the motor.

<img width="450" height="500" alt="Screenshot 2026-09-13 142431" src="https://github.com/user-attachments/assets/31f51d7f-513a-4454-9fbf-c63ed2e664e1" />

<img width="400" height="500" alt="Screenshot 2026-09-13 142450" src="https://github.com/user-attachments/assets/66f66033-d754-42ce-b936-7e41f4948695" />

Finally, I made the bolts for feature 2 using a linear pattern.

<img width="350" height="500" alt="Screenshot 2026-09-13 142714" src="https://github.com/user-attachments/assets/085fd416-91f6-4ffb-bc34-ff50391b5b2c" />

<img width="300" height="500" alt="Screenshot 2026-09-13 142840" src="https://github.com/user-attachments/assets/12949d0e-77e3-4a3b-9349-0ce0f05c976c" />

## Lessons Learned

 - I got a refresher on mass moment of inertia
 - I learned how to use beam bending equations for both stress and deflection
 - I learned how to input equations and tables into github

SolidWorks Links:

<a href="A4 Motor Mount.SLDPRT" download>
    Download SOLIDWORKS Part
</a>
