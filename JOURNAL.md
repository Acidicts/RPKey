---
Title: "PiKey"
Author: "Alex Hayes"
Description: "A Hardware Authentication Key Powered by a rp2350!"
Created On dd/mm/yyyy: "16/08/2025"
---

# June 16th: Decided on using RP2354A!

I looked at the datasheet to decide which chip to use.
I chose a "A" chip as i don't need the amount of pins found on the "B" chips
Later on i decided on a rp2354a I chose a "4" as the use case of the chip shouldn't need more than the onboard storage so to save space i am using on-chip flash

<img width="720" height="175" alt="image" src="https://github.com/user-attachments/assets/c15bf276-5ee5-4040-a7a1-90c571135a46" />

**Total time spent: 0.1h = 6 mins**

# August 16th: Started research!

started to look at example rp2354a schematics and read bits of the datasheet to understand how to create the pcb

<img width="549" height="789" alt="image" src="https://github.com/user-attachments/assets/6a393f00-1f69-4a23-9c1a-12a51857d882" />
<img width="890" height="745" alt="image" src="https://github.com/user-attachments/assets/4d6e996f-3961-4497-a0f7-3efa3b873d18" />

**Total time spent: 0.75h == 45 mins**

# August 17th: Decided on a linear Voltage regulator!

I continued following the hardware design at https://datasheets.raspberrypi.com/rp2350/hardware-design-with-rp2350.pdf
and decided to use the NCP1117ST33T3G instead of the NCP1117-3.3_SOT223

<img width="700" height="422" alt="image" src="https://github.com/user-attachments/assets/ed91af0f-5235-4f5c-aa0e-d197ea0bcc58" />


**Total time spent: 0.5h == 30 mins**


# August 17th: Continued Building up the Schematic!

I continued following the hardware design at https://datasheets.raspberrypi.com/rp2350/hardware-design-with-rp2350.pdf

- Added an external oscillator
- Added USB-C Port with PD configuration for 5V 5.1K resistors
- Added ESD Protection to the Data Lines to the RP2354A
- Added Reset and Bootsel Button
- Added External Flash
- Added a RGB Light
- Added JST Debug Connector
- Added Breakout Pads

<img width="1178" height="826" alt="Schematic_RPKey_2025-08-17" src="https://github.com/user-attachments/assets/46079af5-533d-407b-98a8-6ae7473f382b" />

**Total time spent: 3h == 180 mins**

# August 17th: Started On the PCB Design!

I started layout of the pcb but currently have a road block of my drc check

<img width="342" height="422" alt="image" src="https://github.com/user-attachments/assets/b6c86ffa-3eb7-453a-816e-8a844b4ab07a" />

**Total time spent: 2.5h == 150 mins**

# August 19th: Decided to redo pcb design!

Renaming the Project to PiKey and starting to create a new pcb design
