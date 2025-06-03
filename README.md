# Smart-Curtain-System
This project implements an automated smart curtain system using a double-layer PCB. The system automatically opens/closes curtains based on sunlight, using digital logic circuits, sensors, and motor control.

Here's a breakdown of the components and their roles :

Logic Gates (Core Control Logic) :

7408 (AND Gate) → Checks if both sunlight (LDR) AND curtain position (limit switch) conditions are met.

7432 (OR Gate) → Provides flexibility (e.g., manual override OR automatic operation).

7400 (NAND Gate) → Used for safety (e.g., stop motor if limit switch NAND light condition fails).

NOT Gate (Inverter) → Reverses signals (e.g., converts "dark" to "close curtain" command).

I/O Components :

LDR (Light Sensor) → Detects sunlight intensity → Triggers motor when light crosses a threshold.

Limit Switches → Physical switches at curtain’s open/closed positions → Cut power to motor to prevent overtravel.

Push Buttons (INPUT) → Manual control for testing/debugging logic gates.

LEDs → Visual feedback for gate outputs (e.g., LED ON = logic "1").

Power & Motor Control :

Power Supply Circuit → Regulates voltage for ICs (5V) and motor (12V).

Motor Driver → Amplifies logic signals to drive the high-current curtain motor.

Resistors (R1-R5) → Current limiters for LEDs/sensors (prevents burnout).

PCB Design (Double-Layer) :

Top Layer: Signal traces (logic gates, sensors).

Bottom Layer: Ground/power planes (reduces noise).

In summary , This smart curtain system uses a double-layer PCB with logic gates (AND, OR, NAND), an LDR sensor, and limit switches to automate curtain movement based on sunlight. The motor opens/closes the curtains when light changes, while LEDs and resistors provide feedback. The compact PCB design separates power and signal layers for reliable operation.
Layout: Compact but avoids interference (e.g., motor driver placed far from LDR).
