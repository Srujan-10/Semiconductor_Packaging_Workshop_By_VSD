# Creating Molding Compound in ANSYS Q3D

## Objective:
To encapsulate the DIE, wire bonds, and bond pads in a molding compound to protect the package.

---

## Step-by-Step Instructions:
![Screenshot 2025-05-04 114436](https://github.com/user-attachments/assets/f46c8d1d-ebbb-49dc-943d-aa5dc89c8025)

### 1. Define Molding Compound Dimensions
- Ensure the compound fully encloses the **die**, **bond wires**, and part of the **substrate**.
- Thickness above the die: Typically 0.5 – 1 mm.
- Extend horizontally beyond die and wires for coverage and safety.

---

### 2. Create the Geometry
1. Go to **Modeler → Create → Box** (or **Draw Rectangle → Thicken**).
   ![Screenshot 2025-05-04 114731](https://github.com/user-attachments/assets/9da08c44-e76e-4e8b-ab54-fb064b1d6548)

3. Draw a rectangle covering:
   - Length and width: Larger than the substrate.
   - Height: From the top of the substrate to desired molding height.
![Screenshot 2025-05-04 114909](https://github.com/user-attachments/assets/b39dfff7-5cec-4cdc-bce7-dade988917e7)


![Screenshot 2025-05-04 114918](https://github.com/user-attachments/assets/3db47436-609b-4dae-b43b-35361015e222)\


![Screenshot 2025-05-04 115541](https://github.com/user-attachments/assets/79271b55-baca-49ab-b7c5-bec493df56b7)

4. Subtract the space below the substrate if needed.

---

### 3. Name the Object
- Rename the body to `MOLDING_COMPOUND`.

---

### 4. Assign Material
- Assign the material as **EMC (Epoxy Molding Compound)** or define custom:
   - Relative Permittivity (εr): 3.5 – 4.5
   - Loss Tangent: ~0.02
   - Thermal Conductivity: ~0.8 W/m·K
   - Density: ~1.8 – 2 g/cm³

---

## Notes:
- Ensure molding does not overlap with the bottom of the substrate.
- Avoid merging geometry with wire bonds during boolean operations.

---

## Result:
Your model will now include a protective **molding compound** enclosing the die and wires, completing the basic packaging structure.

