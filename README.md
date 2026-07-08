# Hexapod Robot

<p align="center">
    <img src="Images/Hexapod-Assembled.jpg" width="45%" alt="Hexapod Robot Assembled" />
    &nbsp;
    <img src="Images/Hexapod-CAD-With-Cover.png" width="45%" alt="Hexapod Robot CAD" />
</p>

**Hexapod Robot** is a 6-legged walking robot featuring:

- 6-leg hexapod locomotion design
- 14cm × 19cm × 5.3cm body chassis
- Arduino R4 Minima microcontroller
- MG90S servo motors for leg actuation
- 2× PCA9685 16-channel PWM driver boards
- 300W 20A DC-DC buck converter for power distribution
- Dual 12V 2A power adapters
- 3D printed ABS/PETG chassis and leg components
- Modular leg design for easy assembly and maintenance

## Dimensions

### Body Chassis

- **Width:** 14 cm
- **Length:** 19 cm
- **Height:** 5.3 cm
- **Chassis Weight:** 100-120 grams

### Build Volume

- **Total Height (with legs):** TBD (awaiting leg assembly)
- **Total Footprint:** Approximately 45cm × 50cm (estimated with legs extended)

## Electronics

### Microcontroller
- **Arduino R4 Minima** - Main control board

### Servo Motors
- **MG90S** - Micro servo motors for leg joints
- Total servos required: 18 (3 per leg)
- Torque: 1.8 kg/cm
- Operating voltage: 4.8-6V

### Power Distribution
- **PCA9685 PWM Driver Boards** - 2× units (16-channel each)
- Controls up to 32 servo motors
- Frequency: 24-1600 Hz

### Power Supply
- **DC-DC Buck Converter** - 300W, 20A capacity
- Input: 24V (dual 12V adapters in series configuration)
- Output: Adjustable 3.3V-12V for different components

### Temporary Power
- **2× 12V 2A Adapters** - Currently used for development and testing

## CAD Files

The complete 3D design is available in the `CAD/` directory:

- **CAD/Assemblies/** - Full assembly reference files (STEP format)
- **CAD/Parts/** - Individual 3D printable parts (STL format)

View the CAD designs without panels here:
<img src="Images/Hexapod-CAD-Without-Cover.png" width="50%" alt="Hexapod Robot CAD Without Cover" />

## 3D Printing Guide

All chassis and leg components are designed for FDM 3D printing.

### Recommended Print Settings
- **Layer Height:** 0.2mm
- **Infill:** 40%
- **Support Material:** Required everywhere
- **Print Speed:** 60mm/s for better quality
- **Nozzle Temperature:** 200-220°C (PLA) or 240°C (PETG)
- **Bed Temperature:** 60°C (PLA) or 80°C (PETG)

### Fasteners Required
- **2mm Screws** - For part assembly and securing servo motors

## BOM (Bill of Materials)

| Component | Quantity | Notes |
|-----------|----------|-------|
| Arduino R4 Minima | 1 | Main controller |
| MG90S Servo Motor | 18 | 3 per leg (2 hip, 1 knee) |
| PCA9685 PWM Driver | 2 | 16-channel each |
| DC-DC Buck Converter | 1 | 300W, 20A |
| 12V Power Adapter | 2 | 2A each |
| 2mm Screws | ~50 | Assembly fasteners |
| Jumper Wires | 100+ | Connections |
| Breadboard | 1-2 | Prototyping |

## Project Status

### Completed ✅
- Chassis body design and 3D printing
- Chassis assembly with electronics
- Arduino R4 Minima setup
- PCA9685 PWM boards integrated
- Power distribution system configured
- Electronics testing and validation

### In Progress 🔄
- Leg 3D printing (STL files ready in CAD/Parts/)
- Servo motor calibration
- Leg assembly and mechanical testing
- Gait algorithm development

### Upcoming 📋
- Walking gait implementation
- Autonomous navigation
- Sensor integration (optional)
- Remote control system

## Software Requirements

| Purpose | Software |
|---------|----------|
| Arduino Programming | Arduino IDE or PlatformIO |
| CAD Viewing/Editing | FreeCAD, Fusion 360, or SolidWorks |
| 3D Slicing | Cura, PrusaSlicer, or Bambu Studio |

## Assembly Instructions

### Phase 1: Chassis Assembly (Completed)
1. Assemble 3D printed chassis components
2. Mount Arduino R4 Minima on chassis
3. Install PCA9685 PWM driver boards
4. Connect DC-DC buck converter
5. Wire power distribution
6. Test power and communication

### Phase 2: Leg Assembly (In Progress)
1. 3D print all leg components with recommended settings
2. Clean and assemble printed parts
3. Mount MG90S servos to leg joints
4. Connect servos to PCA9685 boards
5. Calibrate servo angles
6. Attach legs to chassis using 2mm screws

### Phase 3: Programming & Testing
1. Load servo control firmware to Arduino
2. Test each leg individually
3. Implement hexapod gait algorithm
4. Validate walking motion
5. Fine-tune movement parameters

## Notes

- Each leg requires 3 MG90S servo motors (2 hip joints, 1 knee joint)
- Power distribution uses dual 12V adapters for adequate current supply
- PCA9685 boards handle PWM signals for all 18 servos simultaneously
- Modular design allows for easy component replacement and upgrades
- Use appropriate heat dissipation for the buck converter during extended operation

## License

This Hexapod Robot project is open-source. Please refer to the LICENSE.md file for details.

## Credits

- Arduino R4 Minima documentation and community
- PCA9685 PWM driver board reference designs
- Hexapod robotics community and open-source projects

---

**Built with:** 3D printing, Arduino, and servo motors 🤖
