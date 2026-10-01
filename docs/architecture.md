# MiniLab system architecture

**Status: Conceptual architecture for the unbuilt V1 design**

This document separates the local V1 measurement path from optional future connectivity. It describes intended responsibilities, not a completed circuit or implementation.

## V1 local data flow

```text
Physical environment
        ↓
Temperature/humidity sensor and ambient-light sensor
        ↓
ESP32-class controller
        ↓
Reading processing and application state
        ↓
OLED display
```

The physical environment provides conditions to measure. The sensors convert those conditions into electrical readings. The ESP32 reads the sensor interfaces, applies the small amount of processing needed for presentation, handles the physical input, and sends a local view of the measurements to the OLED.

## V1 responsibilities

### Sensors

Provide temperature, humidity, and ambient-light readings using interfaces that will be selected and validated during design.

### ESP32

Coordinate the peripherals, manage timing and application state, react to the button, and handle basic errors. The exact board and GPIO assignments remain unresolved.

### Processing

Convert raw readings into values and statuses that are understandable on the local display. V1 should avoid unnecessary data infrastructure or complex analysis.

### OLED

Provide the primary user-visible output. The first display layout should favor legibility and useful error states over elaborate interaction.

## Optional future data flow

```text
ESP32
  ↓
Wi-Fi/Bluetooth
  ↓
Web application
  ↓
Storage and visualization
```

This path is explicitly future functionality. It could eventually support data logging, remote viewing, or plots, but it would add networking, application, storage, security, and troubleshooting concerns.

## Why V1 avoids the extra path

MiniLab is a first hardware project with an approximate $30 parts target and approximately 10 hours of initial design effort. Keeping V1 local makes the core learning loop visible: connect hardware, read a sensor, handle an input, display a result, and debug the physical system. Wireless communication and web infrastructure can be evaluated after that foundation is understood.
