---
Title: "PiKey"
Author: "Alex Hayes"
Description: "A Hardware Authentication Key Powered by a rp2350!"
Created On dd/mm/yyyy: "16/08/2025"
---

# June 16th:
## Decided on using RP2354A!

I looked at the datasheet to decide which chip to use.
I chose a "A" chip as i don't need the amount of pins found on the "B" chips
Later on i decided on a rp2354a I chose a "4" as the use case of the chip shouldn't need more than the onboard storage so to save space i am using on-chip flash

<img width="720" height="175" alt="image" src="https://github.com/user-attachments/assets/c15bf276-5ee5-4040-a7a1-90c571135a46" />

**Total time spent: 0.1h = 6 mins**

# August 16th
## Started research!

started to look at example rp2354a schematics and read bits of the datasheet to understand how to create the pcb

<img width="549" height="789" alt="image" src="https://github.com/user-attachments/assets/6a393f00-1f69-4a23-9c1a-12a51857d882" />
<img width="890" height="745" alt="image" src="https://github.com/user-attachments/assets/4d6e996f-3961-4497-a0f7-3efa3b873d18" />

**Total time spent: 0.75h == 45 mins**

# August 17th
## Decided on a linear Voltage regulator!

I continued following the hardware design at https://datasheets.raspberrypi.com/rp2350/hardware-design-with-rp2350.pdf
and decided to use the NCP1117ST33T3G instead of the NCP1117-3.3_SOT223

<img width="700" height="422" alt="image" src="https://github.com/user-attachments/assets/ed91af0f-5235-4f5c-aa0e-d197ea0bcc58" />


**Total time spent: 0.5h == 30 mins**


## Continued Building up the Schematic!

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

## Made the PCB Design!

I started layout of the pcb but currently have a road block of my drc check

<img width="342" height="422" alt="image" src="https://github.com/user-attachments/assets/b6c86ffa-3eb7-453a-816e-8a844b4ab07a" />

**Total time spent: 2.5h == 150 mins**

# August 19th:
## Decided to redo pcb design!

Renaming the Project to PiKey and starting to create a new pcb design


## Created 2nd iteration of my PCB Design!

Created new pcb to follow drc requirments

<img width="373" height="474" alt="image" src="https://github.com/user-attachments/assets/5f5df065-e17e-4c80-9eb9-c4806a57f510" />

**Total time spent: 1.5h == 90 mins**

## Changed which usb-c port I use!

Changed usb-c male port used as the footprint didn't include the port shape

<img width="383" height="313" alt="image" src="https://github.com/user-attachments/assets/d8bcc441-1660-465d-bff2-383ad1b61cfd" />


**Total time spent: 0.4h == 24 mins**


## Added some silkscreen art!

Added custom silkscreen art because why not

<img width="597" height="332" alt="image" src="https://github.com/user-attachments/assets/991167f8-f400-4253-b4cb-a5c906164f31" />

**Total time spent: 0.2h == 12 mins**

## Issue with getting screenshot of order!

Unable to create the order due to lack of components

components such as the rp2354a cannot be swapped out as the board is built around it

<img width="1919" height="883" alt="image" src="https://github.com/user-attachments/assets/5c41a9b7-80c9-40c8-9c57-e84a32eccad7" />

# August 21th
## 3rd try is a charm

Decided to restart from the schematic to use the RP2350A instead of the RP2354A due to JLCPCB stock

<img width="1866" height="384" alt="image" src="https://github.com/user-attachments/assets/6a81bce1-449f-4cb2-84c2-cf3302249f49" />

## USB Gender Change

Due to lack of usb-c male connectors i will be using a usb-c female connector
Although this means the device cannot be directly plugged into a device it can be manuvered around said device

♂️➡️♀️

**Total time spent: 0.2h == 12 mins**

# August 22nd
## Started making the schematic

I added
- a Boot Button 
- a flash memory chip
- a crystal oscillator
- decoupling capacitors
- input power supply

<img width="2923" height="2066" alt="Schematic_RPKey_2025-08-22" src="https://github.com/user-attachments/assets/e301a1a2-454e-445b-8f2a-75f683df6d56" />

**Total time spent: 1h == 60 mins**

## Finished Schematic, Started PCB

I finsihed the schematic and then went on to start the pcb

<img width="1604" height="827" alt="Schematic_RPKey_2025-08-22" src="https://github.com/user-attachments/assets/23a7e05e-cb96-4d2f-984a-111c3de5e0dc" />

**Total time spent: 1.5h == 90 mins**

## Finished PCB
I finished the pcb and made it as compact as possible ( as small as I could make it )

<img width="346" height="635" alt="image" src="https://github.com/user-attachments/assets/559d224e-2e45-435b-b972-ca0c7084b68f" />

**Total time spent: 1h == 60 mins**

## Added Silkscreen Decoration

- Added Hacklub Logo
- Added a Custom Secured by Raspberry Pi Logo
- Added a Powered by RP2350A Descriptor

**Total time spent: 0.3h == 18 mins**
