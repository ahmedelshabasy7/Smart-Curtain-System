# Smart-Curtain-System
This project implements an automated smart curtain system using a double-layer PCB. The system automatically opens/closes curtains based on sunlight, using digital logic circuits, sensors, and motor control.
Here's a breakdown of the components and their roles:
Logic Gates (Core Control Logic) :

7408 (AND Gate) → Checks if both sunlight (LDR) AND curtain position (limit switch) conditions are met.

7432 (OR Gate) → Provides flexibility (e.g., manual override OR automatic operation).

7400 (NAND Gate) → Used for safety (e.g., stop motor if limit switch NAND light condition fails).

NOT Gate (Inverter) → Reverses signals (e.g., converts "dark" to "close curtain" command).

