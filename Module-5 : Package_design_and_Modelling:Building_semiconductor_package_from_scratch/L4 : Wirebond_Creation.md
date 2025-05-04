# Creating Wire Bonds in ANSYS Q3D

## Objective:
Connect bond pads on the DIE to the substrate using gold wire bonds.

---

## Step-by-Step Instructions:

### 1. Define Wire Bond Parameters
- **Wire Material**: Gold (Au)
- **Wire Diameter**: Typically 25 µm (adjust as needed)
- **Start Point**: Center of bond pad on DIE
- **End Point**: Corresponding location on substrate pad
- **Shape**: Curved or arched for mechanical reliability
- 
![Screenshot 2025-05-04 022614](https://github.com/user-attachments/assets/63250967-4f80-420e-8aa4-4083c707697a)

---

### 2. Create Wire Geometry
1. Go to **Modeler → Wirebond
2. Draw a polyline from:
   - Start: Center of bond pad
   - Midpoint: Arched position above the DIE
   - End: Substrate pad or designated bond point
3. Name it `WIRE_BOND_1` (increment for more)
4. 
   ![Screenshot 2025-05-04 022647](https://github.com/user-attachments/assets/2a1c215e-d30f-4477-9e96-bb2a64a54594)

   Create and connect all bond pads :
   
   ![Screenshot 2025-05-04 041648](https://github.com/user-attachments/assets/d401d2c5-0af2-46a2-80d6-9d4fcaa89718)

   Final View of Wire bonds connected to bond pads :

   ![Screenshot 2025-05-04 113024](https://github.com/user-attachments/assets/f1c99d3d-de53-4229-8498-692b6fab13bc)

---

### 3. Assign Wire Material
1. Assign **Gold (Au)** as the material.
   - If not available, create a custom material:
     - Name: `Gold`
     - Electrical Conductivity: ~4.1e7 S/m
     - Density: 19.32 g/cm³ (optional)
2. Assign the material to all wire bonds.

---

## Notes:
- Ensure the wire doesn’t touch unintended geometry (avoid short circuits).
- Verify clearance and mechanical flexibility if simulating thermal or stress.
- Repeat the process for all required bond pads.

---

## Example:
```text
Bond Pad → Wire Bond → Substrate Pad
   Au         Gold        Metal
