
# Lifting 2 kg Instead of 1 kg Using the Same Motors with Gears

## 1. Problem Statement
The robotic arm in the previous task was designed to lift a **1 kg** weight. Now, we need to determine if it can lift **2 kg** by using additional **gears**.


---

## 2. Understanding the Torque Requirement
Torque (τ) is calculated as:

    τ = F × r

where:
- F = mg is the force due to gravity,
- g = 9.81 m/s² (acceleration due to gravity),
- r is the arm length.

### Previous Torque (1 kg Case)
For **1 kg**, assuming the load is applied at the farthest point (**15 cm = 0.15 m**):

    F = (1 × 9.81) = 9.81 N

    τ₁ = 9.81 × 0.15 = 1.47 Nm

### New Torque Requirement (2 kg Case)
For **2 kg**, using the same arm length:

    F = (2 × 9.81) = 19.62 N

    τ₂ = 19.62 × 0.15 = 2.94 Nm

Thus, **the torque must be doubled** to lift 2 kg.

---

## 3. How Gears Can Help
A **gear system** can be used to **increase torque** at the expense of **reducing speed**. 

The gear ratio is given by:

    Gear Ratio = τₒᵤₜₚᵤₜ / τᵢₙₚᵤₜ

Since we need to **double** the torque:

    Gear Ratio = 2.94 / 1.47 = 2

This means we need a **2:1 gear ratio** to **double** the torque.

### Gear Selection
- **Motor Gear (Small):** **10 teeth**
- **Arm Gear (Large):** **20 teeth**
- This gives a **2:1 gear ratio**, effectively doubling the torque while **reducing speed by half**.

---

## 4. Possible Issues and Limitations
Using gears introduces some challenges:
1. **Slower Arm Movement**: Since torque is doubled, the speed is **halved**.
2. **Energy Loss**: Gears introduce **friction** and **mechanical inefficiencies**.
3. **Additional Weight**: Gears add extra mass to the arm.
4. **More Complexity**: Additional design adjustments might be needed.

---

## 5. Conclusion
- **Yes**, the same motors can lift **2 kg** if we use a **2:1 gear ratio**.
- The arm will move **slower**, but it will have enough torque to lift the weight.
- If speed is important, a higher-power motor should be considered instead of using gears.
