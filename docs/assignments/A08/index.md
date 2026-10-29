# A8 – Gear Box Design

## Objective

Design a gearbox that can be assembled and disassembled, including an input pinion, output gear, journal bearings, and gearbox. The following information is given:

| Output | Input |
| -------- | -------- |
| rpm = 1100 | rpm = unknown |
| T = 1.25 in*lb | T = unknown |
| shaft ⌀ = 0.25 in | shaft ⌀ = 0.125 in |
| shaft length = 1in | shaft length = 1 in |
| short shaft | power transmission |

## Design of the Shafts

The first thing I need to do is figure out if the shaft diameters are sufficient by solving for the max stress. According to the machinery handbook, the max allowable shear yield strength should be less than 4000 psi for power-transmitting shafts, and less than 8500 psi for short shafts. The shafts are sufficient if the max stress is less than the max allowable shear strength.

<img width="847" height="660" alt="Screenshot 2026-10-28 092606" src="https://github.com/user-attachments/assets/02edd94d-9c05-42c3-a124-7630967e85cb" />

Since both of my calculated stresses were less than the yield stress, I can verify that the shafts are sufficient.

## Design Journal Bearings

<img width="564" height="663" alt="Screenshot 2026-10-28 092614" src="https://github.com/user-attachments/assets/56f87229-c6d9-4b79-94c3-db5ae1a6ad05" />
<img width="685" height="663" alt="Screenshot 2026-10-28 092630" src="https://github.com/user-attachments/assets/9ccfe4ff-adf1-4b53-92c4-cfa450b0e1fd" />

## Sketch

## CAD Model

Journal Bearing for Input Shaft

<img width="671" height="547" alt="Screenshot 2026-10-28 124439" src="https://github.com/user-attachments/assets/8e00558a-3c78-4977-9e1a-e21a9bd4d079" />
<img width="1166" height="692" alt="Screenshot 2026-10-28 124534" src="https://github.com/user-attachments/assets/baf70289-65d8-4e6c-b791-3742cc9c3096" />
<img width="525" height="485" alt="Screenshot 2026-10-28 124543" src="https://github.com/user-attachments/assets/2e765a86-973f-482a-b280-7c1897031ed8" />

Journal Bearing for Output Shaft

<img width="747" height="518" alt="Screenshot 2026-10-28 124732" src="https://github.com/user-attachments/assets/71c59e25-74ca-4eb3-9c9b-2c0b61d2dde7" />
<img width="1221" height="743" alt="Screenshot 2026-10-28 124751" src="https://github.com/user-attachments/assets/7cd064b6-c4df-4650-b9c6-98a1cb117d4f" />
<img width="578" height="490" alt="Screenshot 2026-10-28 124802" src="https://github.com/user-attachments/assets/fc9bac3e-8a1f-48b7-ae61-25865108de04" />


For my gearbox, I need it to be able to assemble and disassemble. I achieved this by creating a snap-fit connection between the top and bottom halves of the gearbox. I figured that a snap-fit connection would be the easiest to design because it requires no extra pieces, such as bolts. For the gearbox, I originally designed the shafts separately from the gearbox, but later on decided that it would be easier to combine the gearbox halves and the shafts into one part.

Gearbox Top

<img width="713" height="602" alt="Screenshot 2026-10-29 060917" src="https://github.com/user-attachments/assets/85164cbd-62bc-4f2c-b215-b77300fd2882" />
<img width="471" height="338" alt="Screenshot 2026-10-29 060125" src="https://github.com/user-attachments/assets/d93bda89-6a9c-4056-87fe-28420b5e94f1" />

Gearbox Bottom

<img width="707" height="505" alt="Screenshot 2026-10-29 060747" src="https://github.com/user-attachments/assets/db42806a-e59b-4a64-b3c5-e932c1d21337" />
<img width="418" height="432" alt="Screenshot 2026-10-29 060811" src="https://github.com/user-attachments/assets/fc78b8b6-2cda-49c4-8c07-87167eab272f" />

Gearbox Assembly

<img width="1001" height="722" alt="Screenshot 2026-10-29 060941" src="https://github.com/user-attachments/assets/6b92493e-c818-4f90-a3ba-94fb0d92ac01" />
<img width="892" height="662" alt="Screenshot 2026-10-29 060956" src="https://github.com/user-attachments/assets/0e2c6991-3ee0-4e64-9da1-2a6ba9115b17" />


## 2157 Students Only

## Lessons Learned

## CAD File

