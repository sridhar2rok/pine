# Pine 🌲 — Indoor IR Transceiver with Temperature Sensor

An open-hardware IoT node for **indoor infrared (IR) control** combined with **ambient temperature sensing**, based on the original [hutscape/pine](https://github.com/hutscape/pine) project.

---

## Overview

Pine is a compact indoor device that can:

- **Receive IR signals** from remote controls (TV, AC, etc.)
- **Transmit IR commands** to control appliances
- **Monitor ambient temperature** using an onboard sensor
- Serve as a smart home bridge for IR-controlled devices

---

## Hardware

| Component | Description |
|---|---|
| MCU | ESP8266 / SAMD21 |
| IR Receiver | TSOP IR receiver |
| IR Transmitter | IR LED |
| Temperature Sensor | Onboard NTC/digital sensor |
| Form Factor | Custom PCB (KiCad) |

Design files are in the `hardware/` directory. BOM is in `bom/`.

---

## Repository Structure

```
pine/
├── firmware/      # Embedded firmware source code
├── hardware/      # PCB schematic and layout (KiCad)
├── bom/           # Bill of Materials
├── design/        # System block diagrams and design docs
├── images/        # PCB renders and assembly photos
└── _examples/     # Example firmware sketches
```

---

## Getting Started

### 1. Hardware

Fabricate the PCB using the KiCad files in `hardware/`. Order components from the BOM in `bom/`.

### 2. Firmware

Flash the firmware from the `firmware/` directory to your board using PlatformIO or Arduino IDE.

### 3. Configuration

Update WiFi credentials and MQTT broker settings in the firmware config before flashing.

---

## Credits

Forked from [hutscape/pine](https://github.com/hutscape/pine) by Sayanee Basu.

## License

MIT
