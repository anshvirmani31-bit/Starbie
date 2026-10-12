# Starbie

<img width="778" height="685" alt="Screenshot 2026-10-11 at 3 57 45 PM" src="https://github.com/user-attachments/assets/7501445a-9da6-4349-9027-ae73a4ae4ca8" />



Starbie is a tiny motion-controlled digital pet: basically a desktop Tamagotchi with minimal gameplay buttons. Instead of pressing controls, you interact with it by physically moving the board.

## What it is

Starbie is designed to sit on your desk or stay in your hand. It reacts to how you handle (tilting it, moving it, shaking it, etc.)

## Why?

This project was for my week one Half-Life. It was the starter project given to us. I added my own touch to it by adding an on/off button. I thought that this could be useful since if you're connecting starbie to a battery back on the go, you may not want it to be constantly draining power, thus, the on/off button.

## How it works

This project includes a handful of parts such as a motion sensor/gyroscope, temperature and humidity sensor, etc. It uses the seeed studio XIAO ESP32-C3 as the brain. It also includes a 0.96 OLED screen for the menu and the firmware found in Starbie.ino allows you to use two of the three buttons to interact with the menu. The only other way to interact with Starbie is to shake it. Starbie takes advantage of the motion sensor to be able to tell when you shake it and it reacts accordingly. If you never interact with starbie it just sits on your desk slowly dying. Starbie also has stats from 0-100 being Joy, Energy, and Fullness. These can be increased or decreased from their starting value based on how you interact with starbie. Starbie is USB-C powered and doesn't have a built in battery meaning it needs to be plugges in to work and register inputs.

## Pictures

Finished PCB

<img width="778" height="685" alt="Screenshot 2026-10-11 at 3 57 45 PM" src="https://github.com/user-attachments/assets/7501445a-9da6-4349-9027-ae73a4ae4ca8" />

Schematic

<img width="414" height="609" alt="Screenshot 2026-10-11 at 11 16 31 PM" src="https://github.com/user-attachments/assets/abca5e7e-9cad-49fa-a33e-a678b7a25f80" />

<img width="802" height="690" alt="Screenshot 2026-10-11 at 11 16 53 PM" src="https://github.com/user-attachments/assets/1af504e2-f52e-4821-9679-ea31fe174012" />

<img width="407" height="290" alt="Screenshot 2026-10-11 at 11 17 33 PM" src="https://github.com/user-attachments/assets/f5a73898-fa0e-4dc0-8f25-015b88184c6b" />

<img width="272" height="232" alt="Screenshot 2026-10-11 at 11 18 23 PM" src="https://github.com/user-attachments/assets/93b7e5a6-418b-4293-bbac-a06b07bd5664" />

<img width="426" height="314" alt="Screenshot 2026-10-11 at 11 19 19 PM" src="https://github.com/user-attachments/assets/388e460c-d0e6-468c-b9fa-fdb6d5581fbd" />

<img width="407" height="387" alt="Screenshot 2026-10-11 at 11 18 08 PM" src="https://github.com/user-attachments/assets/6f25c8e0-a2d8-440b-8b86-caac7d2b9a5c" />

<img width="271" height="252" alt="Screenshot 2026-10-11 at 11 18 36 PM" src="https://github.com/user-attachments/assets/31e10ffd-7571-430e-ac84-18a2b2e0963e" />

<img width="178" height="200" alt="Screenshot 2026-10-11 at 11 18 48 PM" src="https://github.com/user-attachments/assets/cbbec1dd-ba5e-4cea-84ea-867716817bc3" />

<img width="341" height="255" alt="Screenshot 2026-10-11 at 11 19 10 PM" src="https://github.com/user-attachments/assets/c6bb2795-7eed-42a8-8af5-fa130b1d285f" />

## BOM
| Item             | amount | cost USD (ea.) | Link                                                                  |
|------------------|--------|----------------|-----------------------------------------------------------------------|
| XIAO ESP32 C3    | 1      | 13.45          | https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html            |
| 0.96 OLED        | 1      | 2.76           | https://www.aliexpress.com/item/1005006141235306.html                 |
| MPU6050          | 1      | 1.92           | https://www.amazon.ca/gp/product/B0GWX4N5N7?smid=AUV9BWKKX5AP0&th=1   |
| DHT11            | 1      | 3.73           | https://www.aliexpress.com/item/1005009668759587.html                 |
| MX Switches      | 1      | 2.01           | https://www.amazon.ca/gp/product/B0FQ5DDQYK?smid=A3HCNFR52IFXW0&psc=1 |
| Keycaps          | 1      | 1.25           | https://www.amazon.ca/gp/product/B0FX22HS4J?smid=A309HCDL4YKIK6&th=1  |
| 10k Resistor     | 1      | 1.21           | https://www.aliexpress.com/item/1005012176738771.html                 |
| PCB              | 1      | 3.50           | https://www.jlcpcb.com/                                               |
|                  |        |                |                                                                       |
| Total (each kit) | 1      | 30.28          |                                                                       |



## Repository Contents
- `BOM.csv` - Material costs including taxes and shipping
- `BOM.md` - Detailed material costs
- `JOURNAL.md` - Journal entries on what took how long
- `KiCad PCB.kicad_pcb` PCB file
- `KiCad PCB.kicad_sch` PCB schematic file
- `KiCad.PCB.zip` - Gerber and Drill files
- `Starbie.ino` - Firmware/code
