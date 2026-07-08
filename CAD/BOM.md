# Bill of Materials (BOM)

## Electronics

| Component | Quantity | Part Number/Model | Voltage | Current | Cost (USD) |
|-----------|----------|-------------------|---------|---------|------------|
| Arduino R4 Minima | 1 | Arduino R4 Minima | 5V | - | $18-22 |
| MG90S Servo Motor | 18 | MG90S | 4.8-6V | 500mA (stall) | $45-60 |
| PCA9685 PWM Driver Board | 2 | PCA9685 | 5V (logic), 5-6V (servo) | - | $8-12 |
| DC-DC Buck Converter | 1 | 300W 20A Buck Converter | 24V input | 20A max | $15-20 |
| 2200mAh 11.1V LiPo Battery | 1 | 2200mAh 3S LiPo | 11.1V | 2200mAh | $15-20 |
| LiPo Battery Charger | 1 | Balance Charger | - | - | $8-12 |

## 3D Printed Components (Chassis)

| Component | Quantity | File Name | Print Time (est.) | Material Weight (est.) |
|-----------|----------|-----------|-------------------|----------------------|
| Lower Body Panel | 1 | lowerrectangularbodyy.FCStd | 4-6 hrs | 40-60g |
| Upper Body Panel | 1 | rectangularbodytop.FCStd | 4-6 hrs | 40-60g |
| Body Horn Support | 18 | bodyhornsupport.FCStd | 30 min each | 5-8g each |
| Extra Support Part | 6 | extra part 2.0.FCStd | 1-2 hrs each | 8-12g each |

**Print Settings:**
- Layer Height: 0.2mm
- Infill: 40%
- Support: Everywhere
- Material: PETG or ABS recommended
- Nozzle Temp: 240°C (PETG) or 250°C (ABS)
- Bed Temp: 80°C (PETG) or 110°C (ABS)

## 3D Printed Components (Legs - Phase 2)

| Component | Quantity | File Name | Print Time (est.) | Material Weight (est.) |
|-----------|----------|-----------|-------------------|----------------------|
| Coxa (Hip Joint) | 6 | Corex2.0.FCStd | 2-3 hrs each | 15-20g each |
| Femur (Upper Leg) | 6 | Femur2.0.FCStd | 2-3 hrs each | 15-20g each |
| Tibia (Lower Leg/Foot) | 6 | Tibita2.1.FCStd | 1-2 hrs each | 10-15g each |

*Note: Leg components are designed for Phase 2 assembly after chassis completion*

## Fasteners & Connectors

| Item | Quantity | Size/Type | Purpose |
|------|----------|-----------|---------|
| Screws | ~50 | M2 (2mm) | Chassis assembly and servo mounting |
| Jumper Wires | 100+ | Male-to-Male, Male-to-Female | Electrical connections |
| Breadboard | 1-2 | Half-size or Full-size | Prototyping and testing |
| Servo Extension Cables | 18 | Standard 3-pin servo | Servo to PCA9685 connections |
| USB Cable | 1 | USB-C | Arduino programming and power |
| XT60 Connectors | 2 | Male & Female | LiPo battery power connector |

## Optional Components

| Component | Quantity | Purpose | Cost Impact |
|-----------|----------|---------|------------|
| Capacitors (100µF) | 2-4 | Power supply decoupling | Minimal |
| Resistors (470Ω) | 6 | Optional servo signal protection | Minimal |
| Heat Sink | 1 | Buck converter thermal management | $2-5 |
| LiPo Battery Monitor | 1 | Track battery voltage | $3-5 |

## Cost Breakdown (USD)

### Core Electronics & Power - $130-150
| Item | Cost Range |
|------|-----------|
| Arduino R4 Minima | $18-22 |
| 18× MG90S Servos | $45-60 |
| 2× PCA9685 Boards | $8-12 |
| Buck Converter (300W 20A) | $15-20 |
| 2200mAh 11.1V LiPo Battery | $15-20 |
| LiPo Balance Charger | $8-12 |
| **Subtotal** | **$109-146** |

### Additional Costs (Not Included)
| Item | Cost Range |
|------|-----------|
| 3D Printing Filament | $30-50 |
| Fasteners & Connectors | $5-10 |
| **Total Project Cost** | **$144-206** |

## LiPo Battery Information

### 2200mAh 11.1V (3S) LiPo Specifications
- **Capacity:** 2200mAh
- **Voltage:** 11.1V nominal (3 cells × 3.7V)
- **Discharge Rate:** Up to 30-50C
- **Weight:** ~150-180g
- **Flight Time Estimate:** 15-30 minutes continuous operation

### Battery Safety & Charging
- Always use a balance charger (LiPo charger included in BOM)
- Never over-discharge below 3.0V per cell (9.0V total)
- Store at 50-80% charge when not in use
- Charge on fire-safe surface (LiPo bag recommended)
- Disconnect after use to avoid battery drain

### Power Calculation
- Total servo current draw: ~9A (18× MG90S at full load)
- Arduino + PCA9685 current: ~0.5A
- Total: ~9.5A max
- Battery runtime: ~13 minutes at full load

## Assembly Quantity Checklist

### Before Starting Assembly
- [ ] Chassis 3D printed parts cleaned and ready
- [ ] 18× MG90S servos tested
- [ ] Arduino R4 Minima programmed
- [ ] PCA9685 boards tested
- [ ] Buck converter configured for proper voltage output (11.1V input, 6V servo output)
- [ ] LiPo battery fully charged
- [ ] LiPo balance charger ready
- [ ] All jumper wires organized
- [ ] M2 screws counted and sorted

### Chassis Assembly (Phase 1 - Current)
- [ ] 1× Lower body panel
- [ ] 1× Upper body panel
- [ ] Arduino R4 Minima
- [ ] 2× PCA9685 boards
- [ ] Buck converter
- [ ] 2200mAh 11.1V LiPo battery
- [ ] XT60 connector cables
- [ ] Jumper wires and breadboard
- [ ] 18× horn supports
- [ ] 6× extra support parts

### Leg Assembly (Phase 2 - Upcoming)
- [ ] 6× Coxa (Corex)
- [ ] 6× Femur
- [ ] 6× Tibia
- [ ] 18× MG90S servos
- [ ] Servo extension cables
- [ ] M2 screws for assembly

## Important Notes

- **Wireless Operation:** LiPo battery enables truly autonomous hexapod movement
- **Runtime:** 13 minutes continuous, 30+ minutes intermittent operation
- **Charging Time:** 1-2 hours with balance charger (DO NOT fast charge LiPo)
- **Safety:** Always disconnect battery when not in use to prevent accidental drain
- **Storage:** Store battery at 50-80% charge in cool, dry place
- **Replacement:** LiPo batteries degrade over time (typical lifespan: 200-300 charge cycles)
- **Buck Converter Adjustment:** Set output to 6V for servo power (optimal for MG90S motors)
