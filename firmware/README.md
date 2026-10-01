# Firmware

**Status: Planned; no substantial firmware has been implemented.**

The firmware will eventually coordinate the sensors, display, and physical input on the ESP32-class controller. The implementation should remain small and readable so that it supports learning and debugging rather than hiding the hardware behavior behind unnecessary complexity.

## Planned responsibilities

- Initialize the controller and connected peripherals.
- Read temperature and humidity.
- Read ambient light.
- Update the OLED with measurements and useful status information.
- Detect and handle button input.
- Manage a small application state model, such as the default measurement view and an input-driven alternate view.
- Report or display initialization and reading errors.
- Keep timing, retry behavior, and hardware assumptions explicit.

The exact task boundaries and update cadence should be chosen after the components and interfaces are selected.

## Framework and language options

The project has not automatically selected a framework. Two reasonable candidates are:

### Arduino framework / C++

This may provide broad board and library support, many beginner examples, and a direct path to understanding embedded C++ and GPIO. It also introduces more language and toolchain detail.

### MicroPython

This may support quick experiments and an approachable interactive workflow. The trade-offs include different library availability, runtime behavior, and potentially less direct exposure to the conventional compiled embedded workflow.

The choice should consider the learning objectives, selected modules, debugging experience, and available documentation. Record the decision in the engineering journal when it is made.

## Suggested future structure

Once implementation begins, the code can be organized around responsibilities such as:

1. Hardware initialization.
2. Sensor abstraction and reading results.
3. Input handling and debouncing.
4. Application state and timing.
5. Display rendering.
6. Error and diagnostics handling.

This is a planning outline only; it is not a claim that these modules currently exist.
