# Simulink Basics: LED Blinking Simulation in MATLAB

## Introduction

This course introduces you to **Simulink** by designing a basic LED blinking system. It covers:  
- How to use Simulink to create models.  
- Understanding and configuring blocks.  
- Running simulations for LED control.  

By the end of this course, you will understand how to create and simulate basic Simulink models.  

---

## System Overview

This Simulink model simulates an LED blinking system on a Raspberry Pi. The model includes:  
1. **Pulse Generator**: Creates a periodic signal.  
2. **Switch**: Toggles the LED ON/OFF based on the signal.  
3. **Raspberry Pi LED Block**: Represents the physical LED.  
4. **Scope**: Visualizes the generated signal.  

---

## Step-by-Step Guide to Build the Model

### Step 1: Open Simulink  
1. In MATLAB, click on the **Simulink** button in the toolbar.  
2. Select **Blank Model**.  

### Step 2: Add Blocks  
1. Open the Library Browser by clicking on the Library icon in the toolbar.  
2. Drag and drop the following blocks:  
   - **Pulse Generator**: Found under `Simulink > Sources`.  
   - **Switch**: Found under `Simulink > Signal Routing`.  
   - **Raspberry Pi LED**: Found under `Simulink Support Package for Raspberry Pi Hardware`.  
   - **Scope**: Found under `Simulink > Sinks`.  

### Step 3: Connect Blocks  
1. Connect the **Pulse Generator** to the **Switch**.  
2. Connect the **Switch** to the **Raspberry Pi LED** block.  
3. Connect the output of the **Pulse Generator** to the **Scope** for signal visualization.  

### Step 4: Configure Blocks  
1. Double-click the **Pulse Generator** block:  
   - Set `Amplitude` to **1**.  
   - Set `Period (secs)` to **1**.  
   - Click OK.  
2. Double-click the **Switch** block:  
   - Set the threshold value to **0.5**.  
   - Click OK.  
3. Save the model: `File > Save As`, and name it **BlinkLED.slx**.  

### Step 5: Run the Simulation  
1. Click the **Run** button (green triangle) in the Simulink toolbar.  
2. Observe the **LED block** toggling between ON and OFF states.  
3. Open the **Scope** to view the pulse signal.  

---

## Course Exercises

### Exercise 1: Modify the Pulse Generator  
- Change the `Period (secs)` to **2**.  
- Observe how the blinking pattern changes.  

### Exercise 2: Add Another LED  
- Duplicate the **LED block** and connect it to the same **Switch** output.  
- Run the simulation and observe the behavior.

---

## Summary

In this course, you learned:  
- How to build a Simulink model to simulate an LED blinking system
