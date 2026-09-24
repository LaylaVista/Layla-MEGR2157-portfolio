# A5 – Bracket Design

## Objective

Design a bracket that will hold a Uline strap: https://www.uline.com/Product/Detail/S-12925/Poly-Cord-Strapping/Heavy-Duty-Polyester-Cord-Strapping-3-4-x-2500?pricode=WA9239&gadtype=pla&id=S-12925, made out of aluminum 6061-T6 with a safety factor of 4. Conduct stress analysis to determine appropriate dimensions for structural features.
<img width="696" height="663" alt="Screenshot 2026-09-24 075022" src="https://github.com/user-attachments/assets/62e529ff-cbbc-4d94-842c-bce124100cb9" />

## Decide

The Uline strap is 3/4" wide, so I set feature A to be 1" long. I set the force F = 500 lb to keep the calculations simple.

## Stress Analysis

<img width="958" height="463" alt="Screenshot 2026-09-24 075029" src="https://github.com/user-attachments/assets/c648cadb-3a2b-456f-b5ce-add5000e77eb" />
<img width="621" height="665" alt="Screenshot 2026-09-24 075035" src="https://github.com/user-attachments/assets/c1cec5ce-ab1a-4dcd-b44a-c23498ee9e70" />
<img width="1145" height="663" alt="Screenshot 2026-09-24 075042" src="https://github.com/user-attachments/assets/e244efa8-844d-4d08-8e98-edbae0bed411" />


## Deflection Analysis

<img width="427" height="514" alt="Screenshot 2026-09-24 075054" src="https://github.com/user-attachments/assets/373e9a26-f109-4c56-bf5f-2b15fa3578e7" />
<img width="521" height="661" alt="Screenshot 2026-09-24 075059" src="https://github.com/user-attachments/assets/0852f54e-238b-4161-9c3a-9f3dd1aee283" />

## Drawings

<img width="527" height="665" alt="Screenshot 2026-09-24 075107" src="https://github.com/user-attachments/assets/882d68f8-cce7-472d-beca-022c34eb7716" />

## Lessons Learned

 - Governing failure mode: The diameter I calculated for part A using the stress equations was 0.835 in; however, the diameter obtained through deflection was 0.3177 in. For part C, the calculated height due to stress was greater than the height due to deflection. This shows that both the dimensions due to stress and deflection are necessary to make sure the part functions properly.
 - Error propagation: I assumed a lot of dimensions based on the dimensions of the rigid bar beam. I'm worried that I may have used an incorrect dimension, which would lead to incorrect results for parts C, D, and E.
 - Assumption sensitivity: I made a lot of assumptions throughout this process. For example, I assumed that the load distribution across each cross-sectional area was even throughout. 

This assignment took me about 5 hours to complete.

