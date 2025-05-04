# Creating Die Attach Material and Bond pads : 
## Step 3: Create the SUBSTRATE (larger block below die attach)
![Screenshot 2025-05-04 011342](https://github.com/user-attachments/assets/be4bc699-bf7e-48d0-9cd0-d91203f83b60)


1. Create a rectangle with larger dimensions (e.g., 10 mm x 10 mm).
![Screenshot 2025-05-04 012109](https://github.com/user-attachments/assets/f40933e2-d13e-4fb9-bf93-27b58c7454e7)

2. Name this rectangle: `SUBSTRATE`
3. Use Modeler → Surface → Thicken Sheet
   - Thickness = 0.5 mm
4. Position the SUBSTRATE below the DIE_ATTACH so the DIE stack is centered.
   I have changed the color to light RED
   ![Screenshot 2025-05-04 012211](https://github.com/user-attachments/assets/47aa95ba-adf0-4b7f-833b-9b2d49dfb277)



## Final Structure

- Top Layer: DIE (0.2 mm)
- Middle Layer: DIE_ATTACH (0.1 mm)
- Bottom Layer: SUBSTRATE (0.5 mm)
  ![Screenshot 2025-05-04 012741](https://github.com/user-attachments/assets/2882a480-301a-4b0d-bc2d-c4aa43a3971b)

  ## Step 4 : Creation of bond pads for for die and Sustrate
  # Creating Bond Pads in ANSYS Q3D

## Objective:
Create bond pads on top of the DIE for wire bonding or flip-chip connectivity.

---

## Step-by-Step Instructions:

### 1. Define Pad Dimensions
- **Width**: 100 µm (0.1 mm)
- **Height**: 100 µm (0.1 mm)
- **Thickness**: 5 µm (0.005 mm)

> Adjust dimensions if your design requires specific pad size.

---

### 2. Create a Single Bond Pad
1. Go to the **Modeler** tab.
2. Create a **rectangle** on the top surface of the DIE:
![Screenshot 2025-05-04 014715](https://github.com/user-attachments/assets/6a20a932-f7e1-49a8-9fcb-072a31cb47bf)

   - Place it near a corner or edge of the DIE (leave clearance).
   - 
![Screenshot 2025-05-04 015343](https://github.com/user-attachments/assets/f16f3835-95b7-4b7d-b586-f175d66c5792)

4. Name the object: `BOND_PAD_1` for Die 
5. Go to **Modeler → Surface → Thicken Sheet**
   - Set **Thickness** = 0.005 mm (5 µm)
![Screenshot 2025-05-04 015457](https://github.com/user-attachments/assets/c7bbb2aa-00d5-48f3-8b0f-cc2bbb36d74d)
6.In the same way create bond pads on substrate :
![Screenshot 2025-05-04 015635](https://github.com/user-attachments/assets/c1c61ea2-9674-44d1-b1f4-742344f632f9)

![Screenshot 2025-05-04 021026](https://github.com/user-attachments/assets/9b30173f-b98f-4f5b-9ce0-80114df2993c)

View of both bond pads :

![Screenshot 2025-05-04 021058](https://github.com/user-attachments/assets/46df03b4-7ae1-48bc-b5de-4b4042589604)


---

### 3.  Place Additional Pads
1. Create an array or manually place more pads around the DIE surface.
2. Ensure they are evenly spaced and aligned.

---

### 4. Assign Material and Boundary
- Assign **metal** material (e.g., copper or gold) to the bond pads.
- Define **ports or boundaries** if needed for electrical testing/simulation.

---

## Notes:
- Pads must **not overlap** with the DIE edges.
- Ensure good **electrical contact** between bond pads and interconnects.
- You can add **vias or traces** later to connect pads to the substrate or RDL.



Material for bond pads used is copper 



---

