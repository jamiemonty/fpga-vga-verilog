---
layout: home
title: FPGA VGA Driver
tags: fpga vga verilog
categories: demo
---

Welcome to my Verilog FPGA VGA Driver blog!

## VGA Template Design
### Code Design
The template starting code for this project is organised as five files: three design Verilog source files (VGATop.v, VGASync.v, VGAColourCycle.v), one testbench Verilog source file (Testbench.v), and one Xilinx Design Constraints file (Basys3_Master.xdc).

The design splits the generation of the VGA synchronisation signals and the generation of the VGA RGB colour output signals into separate modules. The VGASync module generates standard timings for a 640x480 VGA display. To change the image on screen that the VGA driver displays, only the VGAColourCycle module requires editing or replacing.
### Simulation
A Verilog testbench enables simulation of the template VGA design in Vivado. Some VGA parameters are changed to have smaller values, for simulation purposes. This is useful for two reasons: 1. Simulation time is significantly slower than real-time; 2. VGA timings require a high number of 25 MHz clock cycles before a VGA frame changes and hence before changes in the RGB colour output signal will be observed.
### Synthesis
### Demonstration
## My VGA Design Edit
### Code Design
### Simulation
### Synthesis
### Demonstration
## Markdown Basics
This is a paragraph. Add an empty line to start a new paragraph.

Font can be emphasised as *Italic* or **Bold**.

Code can be highlighted by using `backticks`.

Hyperlinks look like this: [GitHub Help](https://help.github.com/).

A bullet list can be rendered as follows:
- vectors
- algorithms
- iterators

Images can be added by uploading them to the repository in a /docs/assets/images folder, and then rendering using HTML.
<img src="https://raw.githubusercontent.com/melgineer/fpga-vga-verilog/main/docs/assets/images/DigitalRainDev1.png" width="100" height="100">
