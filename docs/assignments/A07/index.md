# A7 – FEA on Bracket

## Objective

Using the bracket model from assignments A4 and A5, optimize the model for stiffness and strength using FEA simulations in SolidWorks. First, change the mesh until the component's results (safety factor, max stress, and max deflection) converge to within 7%, and then change the geometry to optimize strength-to-weight and stiffness-to-weight ratios. The final model must have a safety factor greater than 3 and a max deflection of 0.25mm.

## Mesh

For my FEA analysis, I fixed the top part of my bracket since this part will not move when the load is applied. Then, I added a 1000-pound downward force distributed across the rod, which will be holding onto the strap. I kept this constant throughout all of my simulations. Then I created three different meshes with increasing fineness: Mesh 1 with 9337 elements, Mesh 2 with 19536 elements, and Mesh 3 with 35875 elements. After simulating my original design, I could only get Mesh 2 and Mesh 3 to converge below 7%.

## Design 1

For design 1, I kept the original design that I created in A6. My max stress was much higher than the material's yield strength, making my safety factor well below 3. The area on the model under the most stress was the part that connects the rod to the rest of the bracket. The part where the maximum deflection occurred was at the end of the rod. I knew that if I wanted to increase strength and stiffness, then both of these areas would need to be redesigned. I also need to make the rest of the bracket thicker to increase the safety factor.

<img width="1592" height="855" alt="Screenshot 2026-10-18 105934" src="https://github.com/user-attachments/assets/676f6130-f268-4fcd-ba69-057cbcc3640a" />
<img width="1596" height="807" alt="Screenshot 2026-10-18 105953" src="https://github.com/user-attachments/assets/3a2fc138-2bb6-447b-8df0-8c62a7dc39e6" />

Mesh 1

<img width="1291" height="828" alt="Screenshot 2026-10-18 110108" src="https://github.com/user-attachments/assets/1ffcd566-b066-49bf-bf6d-f7542d92481d" />
<img width="1147" height="785" alt="Screenshot 2026-10-18 110149" src="https://github.com/user-attachments/assets/ca1cf7d2-a9fd-4e6c-8402-e4de3aad59b7" />

Mesh 2

<img width="1102" height="746" alt="Screenshot 2026-10-18 110254" src="https://github.com/user-attachments/assets/f8fc2d4c-9dab-4c3c-b433-64712fd655aa" />
<img width="1172" height="748" alt="Screenshot 2026-10-18 110322" src="https://github.com/user-attachments/assets/69edd64e-3e0d-40f5-9712-1699b6d92401" />

Mesh 3

<img width="1008" height="742" alt="Screenshot 2026-10-18 110400" src="https://github.com/user-attachments/assets/89e09783-da48-426d-b227-a6c70ac2adde" />
<img width="1061" height="742" alt="Screenshot 2026-10-18 110425" src="https://github.com/user-attachments/assets/68a49f66-e268-4a41-a3fe-7049fef7dc0b" />


|   | Mesh 1 | Mesh 2 | Mesh 3 |
| --- | --- | --- | --- |
| Number of elements | 9337 | 19536 | 35875 |
| Max stress | 1.18*10^6 psi | 1.345*10^6 psi | 1.413*10^6 psi |
| Max deflection | 52.63 mm | 53.58 mm | 54.01 mm |
| Mass | 0.12 lb | 0.12 lb | 0.12 lb |
| Safety Factor | 0.0338 | 0.0297 | 0.0282 |


## Design 2

I made all the walls on my bracket thicker, except for the top two cantilever beams, since they had the lowest stress. Then, I designed a triangular piece to hold the bottom rod to reduce the stress in that piece. I also added fillets around parts of the bracket that experienced low stress and around the triangular piece. 

<img width="657" height="611" alt="Screenshot 2026-10-18 113552" src="https://github.com/user-attachments/assets/dc75f7fe-e60f-451c-b0c1-74d972d23046" />
<img width="783" height="688" alt="Screenshot 2026-10-18 113600" src="https://github.com/user-attachments/assets/fa202c7c-84a8-4aa7-9d8f-32a2b682e073" />

Mesh 1

<img width="1008" height="751" alt="Screenshot 2026-10-18 113906" src="https://github.com/user-attachments/assets/348d17f7-c9bd-4fd7-9bb9-a5115e2323ae" />
<img width="988" height="755" alt="Screenshot 2026-10-18 113918" src="https://github.com/user-attachments/assets/ea6c19f2-9343-4573-84b1-763c834170b6" />

Mesh 2

<img width="945" height="681" alt="Screenshot 2026-10-18 114141" src="https://github.com/user-attachments/assets/41e60398-3040-4f2f-99ad-117ceec55f65" />
<img width="870" height="690" alt="Screenshot 2026-10-18 114201" src="https://github.com/user-attachments/assets/7f66d4cb-2e17-483d-b321-1751f549861f" />

Mesh 3

<img width="950" height="717" alt="Screenshot 2026-10-18 114258" src="https://github.com/user-attachments/assets/088f3384-e055-4f06-8b85-3ed3ff5fedc0" />
<img width="882" height="717" alt="Screenshot 2026-10-18 114312" src="https://github.com/user-attachments/assets/f53ca854-cb27-46e7-bf5b-1af01557c48d" />

Adding these features greatly decreased the max stress and deflection; however, the safety factor was still below 3.

|   | Mesh 1 | Mesh 2 | Mesh 3 |
| --- | --- | --- | --- |
| Number of elements | 9337 | 19536 | 35875 |
| Max stress | 3.501*10^4 psi | 3.642*10^4 psi | 3.698*10^4 psi |
| Max deflection | 0.4216 mm | 0.4234 mm | 0.4240 mm |
| Mass | 0.25 lb | 0.25 lb | 0.25 lb |
| Safety Factor | 1.139 | 1.095 | 1.079 |

## Design 3

For my third design, I decided to increase the length of the entire bracket so I could add another piece to hold the opposite end of the rod. I also added fillets around this newly added piece. I also added some holes on the top two cantilever beams at the top of the bracket to help decrease the mass, since these pieces experienced the least amount of stress.

<img width="751" height="661" alt="Screenshot 2026-10-18 121012" src="https://github.com/user-attachments/assets/81f68b01-5ba8-4258-ab14-4ac3c6b4c02e" />

Mesh 1

<img width="862" height="638" alt="Screenshot 2026-10-18 121102" src="https://github.com/user-attachments/assets/9853dfb6-90c8-4608-9e14-800d1ccdd38d" />
<img width="867" height="657" alt="Screenshot 2026-10-18 121135" src="https://github.com/user-attachments/assets/90ed38c2-a597-43c2-9bb3-6a9353acb7dc" />

Mesh 2

<img width="932" height="657" alt="Screenshot 2026-10-18 121158" src="https://github.com/user-attachments/assets/59b24c7c-02d0-4723-b669-1a20c3f6aec8" />
<img width="847" height="607" alt="Screenshot 2026-10-18 121230" src="https://github.com/user-attachments/assets/8a5cc7d0-1a03-484e-8090-8b9c36a538d1" />

Mesh 3

<img width="885" height="622" alt="Screenshot 2026-10-18 121313" src="https://github.com/user-attachments/assets/c6598024-a471-4661-b936-43ede0e44d2e" />
<img width="833" height="611" alt="Screenshot 2026-10-18 121354" src="https://github.com/user-attachments/assets/7cfb36de-7183-4369-9876-5b8d0b8e79f3" />

This piece helped decrease the max stress and deflection. I was able to achieve a deflection of less than .25 mm; however, I was unable to achieve a safety factor of 3.

|   | Mesh 1 | Mesh 2 | Mesh 3 |
| --- | --- | --- | --- |
| Number of elements | 9337 | 19536 | 35875 |
| Max stress | 1.59*10^4 psi | 1.56*10^4 psi | 1.646*10^4 psi |
| Max deflection | 0.1273 mm | 0.1278 mm | 0.128 mm |
| Mass | 0.32 lb | 0.32 lb | 0.32 lb |
| Safety Factor | 2.51 | 2.56 | 2.42 |



## Lessons Learned

 - I learned how to use finite element analysis (FEA) to optimize a design
 - I learned how to use FEA to determine which areas of a design experience the highest and lowest amounts of stress and deflection
 - I learned that you can add triangular cutouts and rounded cutouts on parts of the design that experience a low amount of stress to decrease the weight of a design

I spent about 5 hours on this assignment

## SolidWorks Files

<a href="A7.SLDPRT" download>
    Download SOLIDWORKS Part
</a>
