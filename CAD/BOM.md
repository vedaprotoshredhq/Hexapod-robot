# Bill of Materials (BOM)

## Electronics

| Component | Quantity | Part Number/Model | Voltage | Current | Notes |
|-----------|----------|-------------------|---------|---------|-------|
| Arduino R4 Minima | 1 | Arduino R4 Minima | 5V | - | Main microcontroller |
| MG90S Servo Motor | 18 | MG90S | 4.8-6V | 500mA (stall) | 3 per leg (2 hip, 1 knee) |
| PCA9685 PWM Driver Board | 2 | PCA9685 | 5V (logic), 5-6V (servo) | - | 16 channels each (controls 32 servos total) |
| DC-DC Buck Converter | 1 | 300W 20A Buck Converter | 24V input | 20A max | Adjustable output (3.3V-12V) |
| 12V Power Adapter | 2 | 12V 2A Adapter | 12V DC | 2A | Series connection for 24V input |

## 3D Printed Components

| Component | Quantity | File Name | Print Time (est.) | Material Weight (est.) |
|-----------|----------|-----------|-------------------|----------------------|
| Coxa (Hip Joint) | 6 | Corex2.0.FCStd | 2-3 hrs each | 15-20g each |
| Femur (Upper Leg) | 6 | Femur2.0.FCStd | 2-3 hrs each | 15-20g each |
| Tibia (Lower Leg/Foot) | 6 | Tibita2.1.FCStd | 1-2 hrs each | 10-15g each |
| Body Horn Support | 18 | bodyhornsupport.FCStd | 30 min each | 5-8g each |
| Extra Support Part | 6 | extra part 2.0.FCStd | 1-2 hrs each | 8-12g each |
| Lower Body Panel | 1 | lowerrectangularbodyy.FCStd | 4-6 hrs | 40-60g |
| Upper Body Panel | 1 | rectangularbodytop.FCStd | 4-6 hrs | 40-60g |

**Print Settings:**
- Layer Height: 0.2mm
- Infill: 40%
- Support: Everywhere
- Material: PETG or ABS recommended
- Nozzle Temp: 240°C (PETG) or 250°C (ABS)
- Bed Temp: 80°C (PETG) or 110°C (ABS)

## Fasteners & Connectors

| Item | Quantity | Size/Type | Purpose |
|------|----------|-----------|---------|
| Screws | ~50 | M2 (2mm) | Chassis assembly and servo mounting |
| Jumper Wires | 100+ | Male-to-Male, Male-to-Female | Electrical connections |
| Breadboard | 1-2 | Half-size or Full-size | Prototyping and testing |
| Servo Extension Cables | 18 | Standard 3-pin servo | Servo to PCA9685 connections |
| USB Cable | 1 | USB-C | Arduino programming and power |

## Optional Components

| Component | Quantity | Purpose |
|-----------|----------|---------|
| Capacitors (100µF) | 2-4 | Power supply decoupling |
| Resistors (470Ω) | 6 | Optional servo signal protection |
| Diodes | 2 | Optional reverse polarity protection |
| LED Indicators | 2-3 | Power and status indicators |
| Heat Sink | 1 | Buck converter thermal management |
| Servo Tester | 1 | Optional - for individual servo testing |

## Summary

### Total Component Count
- **Electronics:** 24 items
- **3D Printed Parts:** 39 components
- **Fasteners & Connectors:** 100+ items
- **Total unique parts:** 163+

### Estimated Costs (USD)
- Arduino R4 Minima: $18-25
- 18× MG90S Servos: $45-90
- 2× PCA9685 Boards: $8-12
- Buck Converter: $15-25
- Power Adapters: $10-20
- 3D Printing Materials: $30-50 (filament)
- Fasteners & Connectors: $10-15
- **Estimated Total: $150-240 USD**

## Assembly Quantity Checklist

### Before Starting Assembly
- [ ] All 3D printed parts cleaned and ready
- [ ] 18× MG90S servos tested
- [ ] Arduino R4 Minima programmed
- [ ] PCA9685 boards tested
- [ ] Buck converter configured for proper voltage output
- [ ] All jumper wires organized
- [ ] M2 screws counted and sorted

### Leg Assembly (per leg)
- [ ] 1× Coxa (Corex)
- [ ] 1× Femur
- [ ] 1× Tibia
- [ ] 3× MG90S servos
- [ ] 3× servo horn supports
- [ ] 6-9× M2 screws
- [ ] Servo extension cables

### Chassis Assembly
- [ ] 1× Lower body panel
- [ ] 1× Upper body panel
- [ ] Arduino R4 Minima
- [ ] 2× PCA9685 boards
- [ ] Buck converter
- [ ] 2× 12V power adapters
- [ ] Jumper wires and breadboard
