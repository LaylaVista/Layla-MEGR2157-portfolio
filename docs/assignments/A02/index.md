# A2 – Truss Stress Analysis

## Objective

 - Design a lightweight planar truss using A500 steel or an alternative material.
 - Create free body diagrams (FBDs) for joints and critical pins.
 - Calculate the required cross-sectional area of truss elements with a safety factor.
 - Determine pin sizes based on shear forces with a safety factor.
 - Solve equations symbolically and numerically for both truss and pin design.
 - Estimate the total weight of the truss and pins.
 - Create a CAD model with accurate dimensions and connections.
 - Compare CAD weight predictions with hand calculations.
 - Document key engineering lessons learned from the process.

## Design Constraints

The image below shows the geometric constraints of the truss. The values are given as a = 0.4m, b = 0.3m, and P is any force between 20-30kN. The cross-sectional area of each element needs to be identical, and each pin needs to be identical.

<img width="355" height="239" alt="Screenshot 2026-08-31 144942" src="https://github.com/user-attachments/assets/feda0bd7-f606-4488-bdf7-054ed5e06a08" />

## 2) Design the overall truss geometry

(a)
Firstly, I sketched out a general idea for my truss. I decided to keep the design simple, only adding two additional members. I chose to keep the truss symmetrical to make the calculations easier later on. For P, my first reaction was to use 20kN because it was the smallest possible load, meaning the internal loads would be lighter, and also because 20kN is a nice, even number. Then, I solved for my reaction forces at joints A and B, and finally, solved for the force in each member of the truss.

<img width="1192" height="1705" alt="IMG_E5480" src="https://github.com/user-attachments/assets/2ea33020-20df-40a7-8adb-1b77e23477d4" />
<img width="716" height="647" alt="Screenshot 2026-09-03 061339" src="https://github.com/user-attachments/assets/d1b1fcf9-a4eb-46a7-b058-45b32b76f0fe" />

To find the density of A500 steel, I did a quick Google search and found that the density is 7850kg/m^3. The weight is found through the equation m=density*volume, and the weight turned out to be 4.610kg. 

<img width="1191" height="568" alt="Screenshot 2026-09-03 061358" src="https://github.com/user-attachments/assets/59e9681a-79b8-4cee-92bc-16c93cc3b327" />


(b)
After solving for all internal forces, I need to determine the cross-sectional area of the truss. In the assignment requirements, the safety factor is given as 3.5. To solve for the cross-sectional area, I used the largest internal load, which was 16.02kN. The material is given in the assignment requirements as A500 steel. I acquired the yield strength through Google and decided to go with A500 Steel, Grade C, which is the most common type of A500 steel. After obtaining the cross-sectional area, I determined the dimensions of the cross-sectional area. I decided to keep the cross-section shape as a square to keep the calculations simple.

<img width="1123" height="647" alt="Screenshot 2026-09-03 061347" src="https://github.com/user-attachments/assets/32802d32-1735-40f5-87f8-2b5d452d1037" />

## 3) Determine the cross-sectional area of the connecting pins

The assignment requires that the pins are to be made of hardened tool steel with a yield shear strength of 170 ksi and a density of 0.278 lb/in^3. I found the cross-sectional area using the same equation I used for the truss. I determined that the diameter had to be 8.34mm and the length of the pin had to be twice the thickness of the truss, since the pin has to be able to connect two members of the truss. After finding the dimensions of the pin, I solved for the weight using the equation m = density(volume) x 5, since there are five pins total.

<img width="834" height="646" alt="Screenshot 2026-09-03 061406" src="https://github.com/user-attachments/assets/5f78f2ee-b2f1-4c1f-932c-b280f43f9296" />


## 4) Utilize CAD software to generate a 3D model of the truss

The following images show my truss and pin design from SolidWorks. The truss and the pins are to be designed separately, and the truss needs to be designed in a single part. I maintained the dimensions of 13.3mm x 13.3mm throughout each member of the truss. The pin diameter is 8.34mm and the length is 26.6mm. 

<img width="1166" height="731" alt="Screenshot 2026-09-03 055306" src="https://github.com/user-attachments/assets/2643fe76-b846-490b-ad58-09f948f38ed7" />
<img width="1028" height="700" alt="Screenshot 2026-09-03 055822" src="https://github.com/user-attachments/assets/a8d94bee-e73d-4207-a663-b7a48ed5708e" />

Mass properties for truss:

<img width="266" height="132" alt="Screenshot 2026-09-03 055650" src="https://github.com/user-attachments/assets/e1f3ee25-4b46-4fd3-9a9b-14bad23845b7" />

The mass of the truss using mass properties turned out to be 4507.47grams or 4.507kg. My calculated mass was 4.610kg, meaning my calculated mass was 2.28% off using the percent error equation.

Mass properties for pins:

<img width="263" height="167" alt="Screenshot 2026-09-03 060352" src="https://github.com/user-attachments/assets/ada4ef9f-b96e-4fb7-bf1b-ad7618f921d0" />

The mass for each individual pin on SolidWorks was 11.19grams or 0.01119kg. Multiply that number by 5, and the total weight of all five pins would be 0.05595kg. My calculated mass for all five pins was 0.175kg, meaning my calculated value was about 213% off. 

## 5) Engineering lessons learned

1) I learned how to design a truss on SolidWorks with the correct cross-sectional area after only being given the material type and the load. I also learned how to correctly accomodate for safety factor.
2) I severely underestimated how much time this project would take. I ended up having to restart the entire project because I designed my initial truss incorrectly. I also had a lot of setbacks when it came to solving for the internal forces. I underestimated how much I have forgotten from when I took my Statics class. I think if I had given myself more time, I would have been able to figure out why my calculated pin mass turned out to be so different from the pin mass from SolidWorks mass properties. The next time I do a project like this, I make sure to give myself ample time to complete it.
3) I learned top pay more attention to directions. One of the mistakes I made during this project was that I didn't realize one of the P forces was facing upwards. This caused to me to restart on my truss calculations multiple times.

## Likelihood of Failure Modes in Truss Components

The members of the truss that are most likely to fail are members CE and ED, since they have the highest internal load.

SolidWorks Links:
