# A7 – FEA on Bracket

## Objective

Using the bracket model from assignments A4 and A5, optimize the model for stiffness and strength using FEA simulations in SolidWorks. First, change the mesh until the component's results (safety factor, max stress, and max deflection) converge to within 7%, and then change the geometry to optimize strength-to-weight and stiffness-to-weight ratios. The final model must have a safety factor greater than 3 and a max deflection of 0.25mm.

## Mesh

For my FEA analysis, I fixed the top part of my bracket since this part will not move when the load is applied. Then, I added a 1000-pound downward force distributed across the rod, which will be holding onto the strap. I kept this constant throughout all of my simulations. Then I created three different meshes with increasing fineness: Mesh 1 with 9337 elements, Mesh 2 with 19536 elements, and Mesh 3 with 35875 elements. After simulating my original design, I could only get Mesh 2 and Mesh 3 to converge below 7%.

## Design 1



|   | Mesh 1 | Mesh 2 | Mesh 3 |
| --- | --- | --- | --- |
| Number of elements | 9337 | 19536 | 35875 |
| Max stress and location | Row 1 Col 2 | Row 1 Col 3 | Row 1 Col 4 |
| Max deflection and location | Row 2 Col 2 | Row 2 Col 3 | Row 2 Col 4 |
| Mass | Row 3 Col 2 | Row 3 Col 3 | Row 3 Col 4 |
| Safety Factor | Row 4 Col 2 | Row 4 Col 3 | Row 4 Col 4 |


## Lessons Learned

