---
title: "Electronic Basic"
description: "A comprehensive guide to understanding basic electronic components, atomic theory, and the practice of assembling simple circuits using Ohm's Law."
summary: "Learn electricity concepts from the atomic level to practical LED circuit assembly as preparation for understanding computer architecture."
date: 2023-09-07T16:04:48+02:00
lastmod: 2026-02-14T19:30:00+07:00
draft: false
weight: 810
toc: true
seo:
  title: "Basic Electronics Learning Guide for Beginners | TeknoEdu"
  description: "An easy way to understand basic electronic circuits with complete, systematic, and detailed component explanations."
  canonical: ""
  noindex: false 
---

Understanding **computer hardware** without knowing basic electronics is like learning to drive a car without knowing how the engine works. This chapter will build your foundation before touching complex components like a *motherboard* or *processor*. All digital systems are essentially the manipulation of high-precision electric currents.

---

## 1. Atomic Foundation: The Origin of Electricity

All advanced technology today works by manipulating the smallest particles in the universe. To understand electricity, we must look into the structure of the atom.



[Image of atom structure showing protons, neutrons, and electrons]


* **Atomic Nucleus:** The center of mass consisting of **Protons** (positively charged) and **Neutrons** (neutral).
* **Electrons:** Negatively charged particles that orbit the nucleus.
* **Valence Electrons:** Electrons located in the outermost orbit. Because they are far from the nucleus, their bond is weak and they are easily detached.
* **Electric Current:** Occurs when these valence electrons jump from one atom to another continuously and in one direction due to a potential difference (voltage).

---

## 2. Current Classification: AC vs DC

In the computer world, these two types of current are used side-by-side but for very different purposes.

| Characteristics | AC (*Alternating Current*) | DC (*Direct Current*) |
| :--- | :--- | :--- |
| **Definition** | Alternating current (the direction of electrons changes periodically). | Direct current (electrons flow steadily in one direction from negative to positive). |
| **Main Source** | Wall Outlets/Grid (PLN). | Batteries, Accumulators, Power Supply (PSU), Adapters. |
| **Usage** | Long-distance electricity transmission. | Sensitive digital devices (Laptops, PCs, Smartphones). |
| **Safety** | **High Danger!** Standard voltage is 220V. | **Relatively Safe.** Low voltage (usually 5V - 12V). |

> **Computer Analogy:** The Power Supply (PSU) acts as a "translator" that converts AC from the wall into stable DC to feed internal components.

---

## 3. Main Variables: Voltage, Current, and Resistance

To understand how a circuit works, we can use the **Water Pipe Analogy**:



1.  **Voltage (V):** Measured in **Volts**. This is "Water Pressure." The force that pushes electrons to flow through the cable.
2.  **Current (I):** Measured in **Amperes**. This is "Water Flow Rate." The number of electrons flowing past a point in one second.
3.  **Resistance (R):** Measured in **Ohms (Ω)**. This is the "Pipe Diameter." The property of a material that obstructs or limits the flow of electricity.

---

## 4. Passive Components: The Stability Guardians

Before moving on to active components like transistors, you must know the "Triple Threat" of passive components:

### A. Resistor
Functions to limit electric current. Without a resistor, components like LEDs will burn out because they receive excessive current.
* **Symbol:** Zig-zag line or a small rectangle.

### B. Capacitor (Charge Storage)
Like a small backup water tank. It stores electrical energy temporarily and releases it when the voltage drops.
* **Function in PC:** Ensures the power supply to the *processor* remains smooth despite small fluctuations.


[Image of different types of capacitors: electrolytic and ceramic]


### C. Inductor (Coil)
Stores energy in the form of a magnetic field. Used to filter high-frequency interference (*noise*) so that data signals do not become corrupt or encounter errors.

---

## 5. Ohm's Law: The Rules of Electronics

Ohm's Law is the fundamental formula that connects Voltage, Current, and Resistance. Since mathematical formulas sometimes do not display well on the web, use the text guide below:

### Formula Triangle:
* **V = I x R** (Voltage = Current multiplied by Resistance)
* **I = V / R** (Current = Voltage divided by Resistance)
* **R = V / I** (Resistance = Voltage divided by Current)

### Practical Case Example:
You have a **9 Volt** battery and an LED bulb that can only receive a maximum current of **0.02 Amperes**. How much resistance (Resistor) is needed so the LED doesn't blow out?

**How to Calculate:**
1. Use the formula to find R: **R = V / I**
2. Enter the numbers: **R = 9 / 0.02**
3. The result: **R = 450 Ohms**

---

## 6. Practical Project: Assembling a Series LED Circuit

Let's apply the theory above into a real single-path circuit.

![Electronic Circuit](elektronik.jpeg)

### Tools and Materials List:
1.  **Power Source:** 9V Battery (Power source).
2.  **Control:** Switch (The door to cut/connect the current).
3.  **Protection:** 470 Ohm Resistor (Guard to keep the LED from exploding).
4.  **Output:** LED (Indicator light).
5.  **Medium:** Jumper Wires (The highway for electrons).
---
