# Starbie

<img width="778" height="685" alt="Screenshot 2026-10-11 at 3 57 45 PM" src="https://github.com/user-attachments/assets/7501445a-9da6-4349-9027-ae73a4ae4ca8" />



Starbie is a tiny motion-controlled digital pet: basically a desktop Tamagotchi with minimal gameplay buttons. Instead of pressing controls, you interact with it by physically moving the board.

## What it is

Starbie is designed to sit on your desk or stay in your hand. It reacts to how you handle (tilting it, moving it, shaking it, etc.)

## Why?

This project was for my week one Half-Life. It was the starter project given to us.

## How it works

This project includes a handful of parts such as a motion sensor/gyroscope, temperature and humidity sensor, etc. It uses the seeed studio XIAO ESP32-C3 as the brain. It also includes a 0.96 OLED screen for the menu and the firmware found in Starbie.ino allows you to use two of the three buttons to interact with the menu. The only other way to interact with Starbie is to shake it. Starbie takes advantage of the motion sensor to be able to tell when you shake it and it reacts accordingly. If you never interact with starbie it just sits on your desk slowly dying. Starbie also has stats from 0-100 being Joy, Energy, and Fullness. These can be increased or decreased from their starting value based on how you interact with starbie. Starbie is USB-C powered and doesn't have a built in battery meaning it needs to be plugges in to work and register inputs.

## Repository Contents
- `BOM.csv` - Material costs including taxes and shipping
- `BOM.md` - Detailed material costs
- `JOURNAL.md` - Journal entries on what took how long
- `KiCad PCB.kicad_pcb` PCB file
- `KiCad PCB.kicad_sch` PCB schematic file
- `KiCad.PCB.zip` - Gerber and Drill files
- `Starbie.ino` - Firmware/code
