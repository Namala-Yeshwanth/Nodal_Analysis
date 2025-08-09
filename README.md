# Nodal_Analysis

This repository contains a Jupyter Notebook (`.ipynb`) that performs **Nodal Analysis** for a gas well.  
It generates **Inflow Performance Relationship (IPR)** and **Tubing Performance Relationship (TPR)** curves for different tubing sizes, determines the optimal operating point for each tubing, and analyzes how tubing diameter affects production.

---

## 📌 What is IPR?
**Inflow Performance Relationship (IPR)** describes how the reservoir delivers fluids into the wellbore.  
- It relates **bottom-hole flowing pressure (Pwf)** to the **production rate (Q)**.  
- The IPR curve is controlled by reservoir properties such as permeability, pressure, and fluid characteristics.  
- At high Pwf (near reservoir pressure), flow rate is low; as Pwf decreases, flow rate increases until limited by reservoir capability.

**Inflow Equation**     
        Pe - del_Pr=Pwf

where:  
Pe = Reservoir Pressure  
del_Pr=Pressure drop in reservoir  
Pwf = Bottom-hole flowing Pressure  

## 📌 What is TPR (VLP)?
**Tubing Performance Relationship (TPR)**, also known as **Vertical Lift Performance (VLP)**, describes the pressure losses in the wellbore as fluids travel to the surface.  
- It relates **flow rate** to the **bottom-hole pressure needed** to lift fluids to the surface for a given tubing size.  
- Larger tubing diameters generally result in **lower friction losses**, enabling higher production rates.

**Outflow Equation**
        Pwf - del_Ptbg - del_sl = P_sep

where:  
del_Ptbg = Pressure drop in tubing  
del_sl = Pressure drop in surface lines  
P_sep = separator Pressure  

**Important** In both IPR and TPR equations must be same becuase there should be one pressure at any given node, not two different pressures.

## 📌 What is Nodal Analysis?
**Nodal Analysis** is a systems approach used in petroleum production engineering to evaluate the interaction between the reservoir (IPR) and the wellbore/surface facilities (TPR).  
- **Goal:** Find the **operating point**, where the reservoir’s ability to deliver fluids (IPR) equals the wellbore’s ability to lift them (TPR).  
- This intersection point determines the **expected production rate** and **bottom-hole flowing pressure** for given well and tubing conditions.

---

## 🎯 Why Perform Nodal Analysis?
- To **optimize production rates** by selecting appropriate tubing sizes and surface equipment.
- To **identify flow restrictions** in the reservoir or wellbore.
- To **forecast performance changes** if well conditions (reservoir pressure, tubing size, choke setting) change.
- To **plan workovers or artificial lift installations** for improved recovery.

---

## 📊 What This Notebook Does
1. **Generates IPR curves** using reservoir data.
2. **Generates TPR curves** for multiple tubing diameters.
3. **Plots IPR and TPR curves** to visualize the system.
4. **Determines the operating point** (production rate & bottom-hole pressure).
5. **Compares tubing sizes** to assess their effect on production.

---

## 📈 Result Example
From the analysis, **larger tubing diameters** allow higher production rates by reducing frictional pressure losses in the wellbore.

