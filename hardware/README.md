# Hardware concept

**Status: Early design / not physically built**

MiniLab is currently planned around an ESP32-class development board, environmental sensors, a small OLED display, and at least one physical input. The electronics have not been purchased, assembled, or validated.

## Main elements

- **Controller:** An ESP32 development board is the current controller candidate. The exact board is not selected.
- **Environmental sensing:** A temperature/humidity sensor is planned.
- **Light sensing:** An ambient-light sensor is planned; it may use I2C or an analog input depending on the selected part.
- **Display:** A small OLED is planned for local readings and status.
- **Input:** A push button or similar simple physical input is planned.
- **Prototype platform:** A breadboard and jumper wires are expected for initial experiments.

## Power considerations

The final design must verify the selected board's power input, the voltage required by each module, current requirements, and safe wiring. The design should account for the controller's 3.3 V logic and should not assume that every module is directly compatible. USB power may be convenient during prototyping, but the exact power arrangement remains to be decided.

## GPIO and communication planning

The current conceptual plan is:

- Use a shared I2C bus where the selected display and sensors support it.
- Use a digital GPIO for the button, with the required pull-up or pull-down arrangement.
- Reserve or select a suitable input for an analog light sensor if an analog candidate is chosen.
- Avoid pins with board-specific boot, flash, or other constraints after the exact ESP32 board is identified.

These are planning directions, not final assignments. Pin numbers, I2C addresses, pull-up values, bus topology, and electrical design are not yet validated.

## Before building

- Identify the exact board and modules.
- Read their datasheets and connection guidance.
- Confirm voltage and logic compatibility.
- Confirm power and current requirements.
- Create a real schematic based on the selected parts.
- Record the final pin plan and unresolved risks.

The future schematic documentation area is [hardware/schematic/README.md](schematic/README.md).
