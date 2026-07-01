[CatLaser_Remaining_Parts_1.csv](https://github.com/user-attachments/files/29534614/CatLaser_Remaining_Parts_1.csv)# catLaser
---
A camera watches the room for your cat. When it detects motion, it figures out which direction the cat is moving and swings a laser dot slightly ahead of that movement — so the cat is always chasing something just out of reach rather than sitting on top of it. When the cat is finished it will point the laser at a dropper that will dispense treats. or when the cat disappears for a few seconds, it does a slow sweep to re-bait attention. After three minutes of nothing, it shuts the laser off and parks itself to save battery.
---
Screenshots
---
<img width="745" height="497" alt="image" src="https://github.com/user-attachments/assets/c1983d30-c2fb-4f8b-85c6-bf9a93603607" />
<img width="747" height="445" alt="image" src="https://github.com/user-attachments/assets/501bf2c6-0b9f-427c-b81f-a4392b8f27f7" />

---
Hardware

Microcontroller: ESP32-S3-WROOM-1-N16R8 (Dual-core Xtensa LX7 @ up to 240MHz, 16MB Flash, 8MB Octal PSRAM)
Camera: Taidacent OV2640 2MP, connected via 24-pin 0.5mm FPC ribbon cable + ZIF socket
Power: Single 18650 Li-ion cell, onboard TP4056 charging via USB-C, MT3608 boost converter (stable 5V rail), AMS1117-3.3 LDO (3.3V rail)
Mounting: 3M Dual Lock strips — peel off to charge, click back into the same spot
---
Software
Unfinished(need parts)
---
Bill of Materials
[Uploading CatLaser_RCat Laser Tracker — Remaining Parts to Buy,,,,,,,,
"PCB already assembled by JLCPCB — this list covers everything still needed: off-board hardware, connectors to solder, and enclosure/mounting materials.",,,,,,,,
,,,,,,,,
"IMPORTANT — do this BEFORE first power-up: (1) wire the MT3608 boost module in isolation, measure its output with a multimeter, and trim the pot to exactly 5.0V. (2) With only power connected (no WROOM module seated), probe the +5V and +3V3 test points to confirm both rails are correct. Only then seat the module and flash firmware.",,,,,,,,
,,,,,,,,
Category,Part,Spec / Connection,Qty,Vendor,Buy Link,Est. Price (USD),Status,Notes
Solder yourself — THT,6mm tactile push button (2-pin),"EN reset + BOOT buttons — through-hole, solder into J_EN / J_BOOT footprints",2,Amazon,Buy →,$7.00,Not Ordered,Sold in 10-packs. Already in your parts list — just needs soldering into the board
Solder yourself — THT,2.54mm breakaway pin headers,"Snap to length for servo (×2), laser, camera (FPC ZIF already on board), battery headers",1,Amazon,Buy →,$7.00,Not Ordered,Already in your parts list. Break off the exact count per connector
Camera,Taidacent OV2640 — 24-pin FPC ribbon,"2MP, 24-pin 0.5mm FPC — plugs into the ZIF socket on your PCB",1,Amazon,Buy →,$10.00,Not Ordered,Updated from the 18-pin version. Confirm gold contacts face the correct side before inserting into ZIF socket
Actuators,SG90 micro servo,Pan axis + tilt axis — signal wire to GPIO1 (pan) and GPIO2 (tilt),2,Amazon,Buy →,$9.00,Not Ordered,"Sold in 3-packs — 1 spare. Wire: Signal → pin header pin 1, VCC → pin 2, GND → pin 3"
Actuators,KY-008 laser diode module,"650nm red, <5mW, Class 2 — signal wire to GPIO42",1,Amazon,Buy →,$7.00,Not Ordered,"Confirm <5mW / Class 2 on the listing before buying. Wire: S → pin 1, VCC → pin 2, GND → pin 3"
Power — off-board,18650 protected Li-ion cell,"3.7V nominal, 3000–3400mAh — plugs into the 2-pin battery header",1,Orbtronic,Buy →,$10.00,Not Ordered,Any reputable protected 18650 works. 'Protected' = built-in over-discharge/over-current circuit
Power — off-board,MT3608 boost-only converter module,Steps raw battery voltage (3.0–4.2V) up to stable 5V rail — connects between BATT_RAW header and +5V_BATT header,1,Amazon,Buy →,$8.00,Not Ordered,IMPORTANT: adjust the onboard pot to exactly 5.0V with your multimeter BEFORE wiring into the board
Mounting & Enclosure,3M Dual Lock reclosable strips,"Stick to back of enclosure + wall — pop off to charge, click back into same spot",1,Amazon,Buy →,$15.00,Not Ordered,
Mounting & Enclosure,M3 screw + standoff kit,"PCB → enclosure standoffs, matched to your 4× M3 mounting holes",1,Amazon,Buy →,$10.00,Not Ordered,
Mounting & Enclosure,PLA filament,Pan/tilt gimbal bracket + wall-mount housing,1,—,already have,$0.00,Not Ordered,Already have printer + filament. Budget ~$20 for a fresh spool if running low
Tools,Digital multimeter,Set boost module to exactly 5.0V; verify 3.3V rail before first power-up,1,Amazon,Buy →,$20.00,Not Ordered,Skip if you already own one
,,,,,Estimated Total,$103.00,,
,,,,,,,,
• PLA filament listed at $0 because you already have a printer and filament — budget ~$20 if you need a fresh spool.,,,,,,,,
• The camera has been updated from the original 18-pin breakout to the Taidacent OV2640 24-pin FPC ribbon you chose — make sure the ZIF socket footprint on your PCB matches before ordering.,,,,,,,,
• Status column is a dropdown — click any cell to mark Not Ordered / Ordered / Received as you go.,,,,,,,,
emaining_Parts_1.csv…]()

