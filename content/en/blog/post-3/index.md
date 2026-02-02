---
title: "Hardware Roadmap: Transforming Current into Logic"
description: "A technical guide to building a RISC-V SBC from circuit design to PCB production."
summary: "Learn how to transform electrical flow into arithmetic logic units and design CPU architectures based on RISC-V."
date: 2026-02-03T02:00:00+07:00
lastmod: 2026-02-03T02:00:00+07:00
draft: false
weight: 80
categories: ["Roadmap"]
tags: ["Hardware", "FPGA", "RISC-V", "PCB"]
contributors: ["Wildan FQ"]
pinned: false
homepage: true
seo:
  title: "Hardware Engineer Roadmap - Nusantara Labs"
  description: "From analog and digital electronics to FPGA design, RISC-V computer architecture, and PCB layouting."
  canonical: ""
  noindex: false
---

This roadmap is a continuation of the previous scientific foundations. Here, we will focus on technical applications, ranging from handling physical cables to independently designing complex computer circuits.

### 1. Analog Electronics: Controlling Energy and Physical Signals

Everything in a computer starts with electrical voltage. This stage teaches you how to tame that energy so it can be used to carry information without damaging the device.

- **Basic Electrical Analysis:** Learning how to use a Multimeter to measure voltage and current. You must master Ohm's Law ($V=IR$) to calculate component requirements with precision.
- **Passive Component Characteristics:** Understanding Resistors (current limiters), Capacitors (voltage storage), and Inductors (interference filters). You will learn how these three components stabilize electrical flow.
- **Diodes and Rectification:** Learning how to convert AC current (from the grid) into stable DC current for electronic circuits.
- **Transistors as Switches:** Focusing on BJTs and MOSFETs. You must understand how a tiny pin (*Gate*) can cut or connect large electrical flows. This is the moment where Physics transforms into Logic.



### 2. Digital Electronics: The Language and Logic of Machines

After mastering electrical control via transistors, it is time to assemble billions of those transistors into units that can perform calculations. Here, electricity is no longer viewed as Volts, but as the digits 0 and 1.

- **Physical Logic Gates:** Studying 7400 series Integrated Circuits (ICs) to see how AND, OR, and NOT gates function in the real world.
- **Combinational Circuits:** Learning to build adders (*Adder*) and path selectors (*Multiplexer*).
- **Sequential Circuits (Memory):** Learning to build *Flip-Flops* and *Registers*. This is the stage where you understand how electricity can be "stored" as data.
- **Hardware Description Language (HDL):** Starting with **SystemVerilog**. You will no longer draw wire paths manually but will instead write code that defines the circuit structure within a chip.

### 3. Hardware Prototyping: Bringing Logic to Life with FPGA

Before creating a permanent chip, you need a virtual "laboratory." An FPGA (Field Programmable Gate Array) allows you to create a "custom chip" that can be reprogrammed repeatedly without the risk of physical damage.

- **Introduction to the FPGA Ecosystem:** Understanding the difference between microcontrollers vs. FPGAs. Studying internal FPGA structures such as *Look-Up Tables* (LUT), *Flip-Flops*, and *Interconnects*.
- **Implementing Logic on Silicon:** Learning to use *Toolchains* (Vivado, Quartus, or Yosys) to convert SystemVerilog code into a *bitstream* sent to the FPGA chip.
- **Simulations and Testbenches:** Learning how to test hardware designs on a computer before running them on actual hardware to ensure there are no logic errors (*bugs*).
- **Hardware Debugging:** Learning to use a *Logic Analyzer* (both physical and virtual) to view the flow of 0s and 1s moving at high speeds inside the chip in real-time.



### 4. Computer Architecture: Designing the Brain and System (RISC-V)

This is the pinnacle of hardware engineering. You use the FPGA as a medium to build the CPU architecture that will serve as the brain of your Single Board Computer (SBC).

- **Instruction Set Architecture (ISA):** Learning the "dictionary" of commands the machine understands, specifically **RISC-V**. You will learn how commands like "Add" or "Store" are translated by the hardware.
- **RISC-V Core Implementation:** Writing or implementing a RISC-V CPU design into the FPGA. At this stage, you will see your custom CPU execute its first instructions (such as toggling an LED via machine code).
- **Datapath and Control Unit:** Learning to design the data traffic paths inside the CPU and the control unit that acts as the traffic police within the chip.
- **Pipelining and Cache:** Studying ways to speed up CPU performance so it can process multiple data points simultaneously without experiencing bottlenecks.



### 5. Systems Engineering and Physical Production (PCB)

Once the computer's brain (RISC-V) has been successfully tested on the FPGA, you must place it on a physical circuit board that is durable, safe, and efficient enough to be used as a standalone device.

- **Power Delivery Management:** Learning how to step down battery voltage into ultra-stable micro-voltages for the processor core using voltage regulators.
- **PCB Layouting (High-Speed Design):** Using software like **KiCad** or **Altium**. You will learn to draw copper traces while maintaining signal integrity to prevent data corruption at high frequencies.
- **System Integration:** Understanding connection standards such as USB, PCIe, and RAM slots so your custom hardware can "talk" to other devices worldwide.
