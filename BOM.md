# MiniLab initial bill of materials

**Status: Planning / candidate list**

This is an initial design aid, not a purchase list or final bill of materials. MiniLab has not been built, and the parts below have not been selected, purchased, or validated.

## Target budget

**Approximate parts target: <= $30**

Prices are marked `TBD` because they have not been researched for a specific seller, date, or shipping situation. The target is a planning constraint, not a confirmed quotation.

| Component | Purpose | Quantity | Candidate / model | Estimated price | Status | Notes |
|---|---|---:|---|---|---|---|
| ESP32 development board | Main controller and future connectivity option | 1 | ESP32-class development board; exact board TBD | TBD | Candidate | Confirm USB/power arrangement, exposed GPIO, 3.3 V logic, and beginner documentation. |
| OLED display | Local display of readings and simple status | 1 | Small I2C OLED module; size/controller TBD | TBD | Candidate | Confirm supply voltage, logic levels, I2C address, and library support. |
| Temperature/humidity sensor | Environmental measurements | 1 | Beginner-friendly digital sensor; exact model TBD | TBD | Candidate | Compare interface, accuracy claims, power needs, library support, and availability. |
| Ambient-light sensor | Ambient light measurement | 1 | Digital I2C or analog light sensor; exact model TBD | TBD | Candidate | The interface affects GPIO planning and firmware complexity. |
| Push button or other input | Basic user interaction | 1 or more | Momentary push button; exact part TBD | TBD | Candidate | Determine whether an internal or external pull-up/down is appropriate. |
| Breadboard | Temporary circuit assembly | 1 | Beginner-friendly solderless breadboard; size TBD | TBD | Candidate | Confirm that it can accommodate the selected modules and wiring. |
| Jumper wires | Breadboard connections | 1 set | Breadboard jumper wire set; type TBD | TBD | Candidate | Wire type and connector compatibility depend on the chosen modules. |
| Resistors / supporting components | Pull-ups, current limiting, or other circuit support | As needed | Values and quantity TBD after design | TBD | Candidate | Do not finalize until the selected modules and schematic establish the need. |
| Enclosure/prototyping material | Later physical protection and mounting | As needed | Cardboard, laser-cut, 3D-printed, or other simple material; TBD | TBD | Future candidate | Enclosure material and cost depend on the CAD approach and final dimensions. |

## Selection criteria

Final component selection should consider:

- ESP32 voltage compatibility and 3.3 V logic.
- Sensor communication interface and whether it fits the chosen GPIO plan.
- Availability from a source that can be checked before purchase.
- Documentation quality and library support.
- Beginner friendliness and ease of debugging.
- Price within the approximate budget.
- Power requirements and safe supply arrangements.
- Physical compatibility with a breadboard and eventual enclosure.

## Verification checklist

- [ ] Identify candidate part numbers and reliable sources.
- [ ] Confirm datasheets and operating-voltage requirements.
- [ ] Confirm logic-level compatibility with the selected ESP32 board.
- [ ] Confirm interfaces, addresses, and pull-up requirements.
- [ ] Record current prices and shipping assumptions.
- [ ] Recalculate the provisional total before purchase.
- [ ] Update this document when a candidate becomes a confirmed design choice.
