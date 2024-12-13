# Handmade Processor Project
_What I cannot create, I do not understand._ – Richard Feynman

## Overview
A documentation repository for the design and development of a custom, programmable processor. This repository documents the journey from initial concepts to a fully functional processor, featuring:

- Basic CPU functionalities.
- A small display for visual output.
- Input/output capabilities (e.g., keyboard connection).
- Expandability for future upgrades.

This is a hands-on project, aiming to create a practical, educational, and expandable system.

## Current Status
- Stage: Planning and research phase.
- Focus: Compiling a roadmap, researching components, and defining initial design requirements.
- Next Steps: Development of a basic architecture diagram.

## Goals
- Design and build a functional processor capable of executing basic instructions.
- Include visual output via a small pixel-based display.
- Implement input/output capabilities, such as a keyboard or other extensions.
- Develop an assembly-like language and a custom higher-level language with a compiler.
- Ensure the system is expandable for future upgrades and additional features.

## Key Features (Planned)
- CPU: Basic processor design, including an ALU, control unit, and registers.
- Memory: Integration of RAM for temporary data storage.
- Display: A compact pixel-based screen for output visualization.
- I/O Capabilities: Ports for external devices, such as a keyboard or sensors.
- Programming: Support for an assembly-level language (low-level programming specific to the processor) and the development of a custom higher-level language with a compiler for ease of use.

## Development Roadmap
The project will follow a structured development process, divided into several key phases: The Roadmap will be updated as the project progresses.

1. Research Phase:
  - Component Requirements:
    - Identify essential components for the CPU (ALU, control unit, registers).
    - Research available RAM chips or alternatives for memory.
    - Explore small display options with manageable interfacing (e.g., SPI/I2C displays).
    - Investigate I/O hardware for peripherals like keyboards or sensors.
  - Component Availability:
    - Check the availability of components from local and online suppliers.
    - Compare prices and practicality for prototyping (e.g., prefer DIP packages for breadboards).
  - Power Requirements:
    - Research the power needs of identified components.
    - Investigate regulated power supplies compatible with breadboard setups.
  - Prototyping Hardware:
    - Evaluate breadboards, jumper wires, and other prototyping tools.
    - Look into logic analyzers or oscilloscopes for testing and debugging.
2. Design Phase:
  - Development of a basic architecture diagram.
  - Definition of an instruction set for the processor.
  - Plan connections for memory, display, and input/output components.
3. Programming Phase:
  - Implementation of an assembly-like language.
  - Development of a compiler for a higher-level programming language.
  - Develop an emulator to simulate the processor’s behavior, including the instruction set and basic components.
  - Test the emulator with sample programs to validate the instruction set and control logic.
  - Refine the assembly-like language based on testing results.
  - Begin development of a compiler for a higher-level programming language to simplify programming.
4. Build Phase:
  - Assembly of components on breadboards as a first prototype.
  - Integration of the display and input/output system.
5. Testing and Debugging:
  - Validation of individual components and the integrated system.
  - Iterative improvements and feature expansions.

## Progress Tracking
Updates will be recorded to reflect the current stage of development, key milestones, and any design changes made during the project.

## Future Directions
Planned expansions and enhancements include:
Future directions will be added as the project progresses.

## Questions
- What is the most practical way to implement RAM?
- Which display resolution strikes a balance between simplicity and functionality?
- How can the processor be designed for expandability and future upgrades?
- What programming language should be used for the compiler development?
- How can the system be optimized for speed and efficiency?
- How to design with power loss and data integrity in mind?