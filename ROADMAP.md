# MiniLab roadmap

**Current status: Phase 0 — Research and design**

The checkboxes below describe planned work. An unchecked item is not evidence that the corresponding hardware or software exists.

## Phase 0 — Research and design

- [ ] Clarify the V1 measurement and interaction requirements.
- [ ] Compare candidate ESP32 boards and sensor modules.
- [ ] Check voltage, power, interfaces, addresses, and documentation.
- [ ] Establish a provisional GPIO and wiring plan.
- [ ] Update the candidate BOM with researched prices.
- [ ] Choose the initial firmware framework deliberately.

## Phase 1 — ESP32 bring-up

- [ ] Obtain the selected development board.
- [ ] Set up the development environment.
- [ ] Run a minimal board bring-up example.
- [ ] Record the board, toolchain, wiring, and observed results in the journal.

## Phase 2 — First sensor

- [ ] Select one temperature/humidity sensor.
- [ ] Read its datasheet and wiring requirements.
- [ ] Prototype one sensor reading.
- [ ] Record successful and failed experiments, if any.

## Phase 3 — OLED/display

- [ ] Select an OLED module and confirm its interface.
- [ ] Prototype display initialization.
- [ ] Show a simple sensor value and a clear error state.

## Phase 4 — Additional sensor/input

- [ ] Add the ambient-light sensor.
- [ ] Add the physical button or other input.
- [ ] Confirm the combined GPIO and bus plan.
- [ ] Document any pull-ups, debouncing, or analog-input considerations.

## Phase 5 — Firmware integration

- [ ] Define the application states and update flow.
- [ ] Integrate sensor reads, display updates, and input handling.
- [ ] Add basic error handling and useful diagnostics.
- [ ] Keep timing and responsibilities understandable for a first project.

## Phase 6 — Enclosure/CAD

- [ ] Measure the assembled prototype after the electronics exist.
- [ ] Choose a simple enclosure approach.
- [ ] Design access for the display, input, power, and sensors.
- [ ] Document design assumptions and revisions.

## Phase 7 — Testing and documentation

- [ ] Define repeatable checks for each sensor and interface.
- [ ] Test power-up, normal readings, input behavior, and visible errors.
- [ ] Record actual observations without inventing precision or results.
- [ ] Finalize the schematic and BOM based on the built design.
- [ ] Document limitations and next improvements.

## Future versions

- **V2 — Data logging:** Save measurements for later review.
- **V3 — Wireless communication:** Explore Wi-Fi or Bluetooth transfer.
- **V4 — Web dashboard:** Plot measurements over time in an optional web application.
- **V5 — Expanded scientific instrumentation:** Add more sensors and experiment modes.

These are future directions, not current implemented features or commitments.
