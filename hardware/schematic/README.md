# Schematic

**Status: No schematic has been created yet.**

This directory is reserved for the future MiniLab schematic and related design exports. A schematic should be added only after the component choices, power arrangement, and pin plan have been researched. This README is not a substitute for a circuit diagram.

## Schematic preparation checklist

- [ ] Identify the exact ESP32 development board.
- [ ] Identify the exact sensor and display modules.
- [ ] Show all power rails and their sources.
- [ ] Show a common ground connection.
- [ ] Verify voltage compatibility for every module.
- [ ] Record GPIO assignments and board-specific constraints.
- [ ] Record I2C addresses and check for conflicts.
- [ ] Determine pull-up requirements and where they are provided.
- [ ] Review the relevant sensor and display datasheets.
- [ ] Check current and power requirements.
- [ ] Review the circuit before wiring the prototype.

When a schematic exists, it should include the selected part identifiers, connection labels, relevant notes, and a revision or date. Do not treat a wiring sketch as a validated electrical design without checking it against the datasheets.
