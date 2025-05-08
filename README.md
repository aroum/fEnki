# fEnki  
fEnki is an open source (free) version of Enki (gbEnki).
fEnki is fully compatible with gbEnki. You can use gbEnki [cases, plates](https://github.com/aroum/gbEnki) and [firmware](https://github.com/aroum/zmk-gbEnki) on your fEnki.

Gerber files can be downloaded in the [releases section](https://github.com/aroum/fEnki/releases).

![Preview](https://github.com/aroum/gbEnki/raw/main/pics/gbEnki_1.jpg)  

Actually, the photo is of gEnki, as soon as gEnki is assembled I will update the photo.

---

## Main Features:  
* 42/36 switches
* Easily accessible power switch and reset button 
* Bluetooth support
* 3 status LEDs
* Double sided board design
* Choc spacing

---
## BOM:  
### Electronic components:
| Component         | Model        | Qty (42-key) | Qty (36-key) |
| ----------------- | ------------ | ------------ | ------------ |
| Reset Button      | SMD 3x4x2mm  | 2            | 2            |
| MCU               | nice!nano v2 | 2            | 2            |
| Diodes            | 1N4148WS T4  | 42           | 36           |
| Power Switch      | BSI-10H      | 2            | 2            |
| Battery           | 301230       | 2            | 2            |
| LEDs              | SMD 0603     | 6            | 6            |
| Resistors         | 0603 1–10k   | 6            | 6            |
| Keyboard Switches | Choc v1      | 42           | 36           |
| Sockets           | PH3.5        |

### Mechanical parts:
| Component        | Model      | Qty (42-key) | Qty (36-key) |
| ---------------- | ---------- | ------------ | ------------ |
| PCBs             | 1.6        | 2            | 2            |
| Cover PCBs       | 0.8-1.6    | 2            | 2            |
| Spacers          | m2x8+      | 4            | 4            |
| Screws           | m2x4 T5*   | 12           | 12           |
| Screws           | m2x5 T5*   | 8            | 8            |
| Nuts             | m2         | 12           | 12           |
| Bumpons          | 5x2mm      | 14           | 14           |
| Magnets for case | disc 7x2mm | 8+           | 8+           |

 *If you are doing a plate assembly you need screws 1mm longer

 [IBOM](https://htmlpreview.github.io/?https://github.com/aroum/fEnki/blob/master/pcb/ibom.html)
---

## Assembly Instructions

### 1. Solder the Diodes

Solder all diodes except the thumb cluster diodes on the **top side** of the PCB. The thumb cluster diodes are slightly elevated and should be soldered on the **bottom side**.
All diodes must face the same direction: align the stripe on the diode body with the stripe on the PCB silkscreen (or with the round pad if the stripe is not visible).

### 2. Solder the LEDs

Solder the LEDs on the **top side** of the PCB.

### 3. Solder the Resistors

Solder resistors on the **bottom side** of the PCB. You can replace them later if you find the LEDs too bright.

### 4. Solder the Reset Button

Mount and solder the reset button on the **top side**.

### 5. Solder the Power Switch

Solder the toggle switch on the **top side**. It's recommended to solder the legs from both sides for durability. Clip off any excess legs.

### 6. Solder the Hotswap Sockets

Solder the sockets. Optionally, you can sand the socket edges for a cleaner look. Clip off any protruding legs.

### 7. Solder the Jumpers

Solder the jumpers on the **bottom side**, near the sockets and power switch. If you're struggling with this step, reduce the soldering temperature to around 200–250°C.

### 8. Solder the TRRS Jack (Optional)

Only if needed — mount and solder the TRRS connector.

### 9. Install and Solder the Microcontroller

Insert male pin headers into the sockets, place the microcontroller on top, clip the protruding legs, then solder.

### 10. Clean the Board

Remove the microcontroller and thoroughly clean the PCB.
If the reset button or switch is not working properly, apply isopropyl alcohol inside, click the button repeatedly, then blow it out.
At this point, you can test the circuit by shorting key pins with tweezers.

### 11. Solder the Switches

Mount and solder the switches. Clip off any protruding legs.
Optionally, screw in mounting screws and secure them with nuts. Depending on the switch model, screws may get slightly stuck between switches — this is generally not an issue.

### 12. Connect the Battery

Solder the battery, observing correct polarity. You can secure it with double-sided tape.

### 13. Final Cleaning

Do a final cleaning of the PCB.

### 14. Flash the Firmware and Bootloader

Flash the firmware. Flashing the bootloader is optional — it is only required to enable LED blinking during boot mode.

### 15. Assemble the Case

Screw the PCB into the case. Optionally, install magnets and rubber feet.
If nuts don’t fit into the slots, you can pre-thread them onto a screw, insert into the slot, heat with a soldering iron, then unscrew. If nuts are loose, use a small drop of super glue.

### 16. Attach Standoffs

Secure the standoffs to the case.

### 17. Attach the Cover

Mount and secure the case cover.

### 18. Install Keycaps

Place the keycaps onto the switches. Done!

---

