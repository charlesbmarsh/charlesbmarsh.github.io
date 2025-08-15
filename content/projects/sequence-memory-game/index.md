---
title: "STM32 LED Sequence Memory Game"
date: 2024-03-01
draft: false
description: "Embedded Systems Project: Simon Says game implemented on STM32 microcontroller with 12-LED matrix, keypad input, and LCD display for an interactive memory challenge."
image: "/led-game.png"
tags: ["Embedded Systems", "C"]
---

**Embedded Systems Final Project** | Cal Poly

[**Youtube Demo**](https://www.youtube.com/watch?v=FXmU54PPUjQ)

## Project Overview
Implemented a Simon Says memory game inspired by humanbenchmark.com, featuring a 3x4 LED matrix that displays increasing sequence patterns for players to replicate using a keypad. The game progressively increases difficulty with longer sequences and faster timing, testing memory skills while demonstrating embedded systems knowledge.

## Technologies Used
- **C** Programming with STM32 microcontroller
- **I2C & SPI** communication protocols
- **STM32CubeIDE** development environment

## Hardware Diagram
<div style="text-align: center;">
    <img src="/led-game.png" alt="LED Game Hardware Diagram" style="border: 2px solid #ddd; border-radius: 8px; padding: 10px; box-shadow: 0 2px 4px rgba(0,0,0,0.1); max-width: 100%; height: auto;">
</div>

## Hardware Components
- **STM32 Nucleo Microcontroller**: Rented from CPE department, ARM Cortex-M4 processor
- **4x3 Keypad**: 12-button matrix for user input (1-9, *, 0, #)
- **MCP23017 I2C I/O Expander**: Controls 12-LED matrix via I2C communication
- **12 LEDs**: Arranged in 3x4 matrix with 150Ω current-limiting resistors
- **LCD Display**: 16x2 character display for game instructions and scoring
- **Jumper Cables**: Custom wiring for component interconnection
- **USB-A to USB-mini**: Power and programming interface


## Learning Outcomes
- **Embedded Programming**: Deep understanding of C programming for the STM32 microcontroller programming and HAL library usage
- **Hardware Interfacing**: Experience with I2C, GPIO, SPI, timers, and peripheral management

This final project for my embedded systems class demonstrates the practical application of embedded systems concepts in creating engaging, interactive applications that combine hardware and software effectively. The project showcases comprehensive understanding of microcontroller programming, communication protocols, and user interface design principles.
