# Transformerless-5V-PSU
A compact transformerless AC-to-DC power supply designed using a capacitive dropper, bridge rectifier, zener protection, and LM7805 voltage regulator.  This project was built to understand low-power offline power supply design and mains-side electronics.

## Features
- 230V AC input
- Capacitive current limiting
- Full-wave bridge rectification
- Ripple filtering
- Zener overvoltage protection
- Regulated 5V DC output
- LED power indication

| Component    | Purpose            |
| ------------ | ------------------ |
| X2 Capacitor | Current limiting   |
| 1N4007       | Rectification      |
| LM7805       | 5V regulation      |
| Zener Diode  | Voltage protection |

⚠ WARNING:
This circuit is non-isolated from AC mains.
Do NOT touch while powered.
Do NOT connect directly to a computer USB port.
Only for educational and experimental purposes.
