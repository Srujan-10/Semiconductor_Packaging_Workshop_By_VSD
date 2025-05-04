# Creating the die and substrate in ANSYS_ELECTROPNIC_DESKTOP
---

## Die and Substrate Creation in ANSYS Q3D Extractor

## Step 1: Create the DIE (3mm x 3mm x 0.2mm)

1. Open ANSYS Q3D and go to the Modeler tab.
2. Select Create → Rectangle.
   ![Screenshot 2025-05-04 002110](https://github.com/user-attachments/assets/21262541-d13d-4b4d-a66c-fb62606ac5cd)

4. Set dimensions:
   - Width = 3 mm
   - Height = 3 mm
 ![Screenshot 2025-05-04 002158](https://github.com/user-attachments/assets/c8c057c8-0479-4305-bdc8-da8df2ad6c69)

5. Name the rectangle: DIE
6. Go to Modeler → Surface → Thicken Sheet


8. Select the DIE and set:
   - Thickness = 0.2 mm
  ![Screenshot 2025-05-04 003257](https://github.com/user-attachments/assets/98b3244a-12ea-4550-828e-ec6b7d38bdf1)
Assign Material as silicon

![image](https://github.com/user-attachments/assets/3004df71-74bd-4b9a-8d9f-bdd7b3f2dcb7)

I have changed the color to light blue .
    
9. Click Apply to complete the die block.

---

## Step 2: Create the SUBSTRATE (Base block under the die)

1. Go to Create → Rectangle again.
   ![Uploading Screenshot 2025-05-04 002423.png…]()

3. Set dimensions larger than the die (for example: 5 mm x 5 mm).
   ![Screenshot 2025-05-04 005805](https://github.com/user-attachments/assets/8ff36fd1-f34b-4238-8ceb-71a2db178641)

5. Name the rectangle: SUBSTRATE
6. Use Modeler → Surface → Thicken Sheet and set:
   - Thickness = 0.5 mm
     ![Screenshot 2025-05-04 010348](https://github.com/user-attachments/assets/837c8160-94f9-4ed1-ab68-3ebab062cea7)
     I have changed the color of substrate to Yellow.

7. Make sure the substrate is placed below the die so the die sits centered on it.

---

Result: Both the die and substrate are now created and ready for further simulation steps like material definition, meshing, and thermal or electrical analysis.

