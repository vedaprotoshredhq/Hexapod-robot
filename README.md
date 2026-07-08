# Hexapod Robot

<p align="center">
  <img src="Images/Hexapod-Assembled.jpg" width="45%" alt="Hexapod Robot Assembled" />
  &nbsp;
  <img src="Images/Hexapod-CAD-Without-Cover.png" width="45%" alt="Hexapod Robot without panels" />
</p>

**Hexapod Robot** is a 6-legged walking robot featuring:

- 14cm × 19cm × 5.3cm body chassis
- Arduino R4 Minima microcontroller
- 18× MG90S servo motors for leg actuation
- 2× PCA9685 16-channel PWM driver boards
- 300W 20A DC-DC buck converter
- 2200mAh 11.1V LiPo battery for autonomous operation
- 3D printed chassis and leg components
- Modular hexapod kinematics for six-legged locomotion

## Dimensions

### Travel area

- **Body Width**: 14 cm
- **Body Length**: 19 cm
- **Body Height**: 5.3 cm

### Body Specifications

- **Chassis Weight**: 100-120g _(body only)_
- **Battery Runtime**: 13-30 minutes _(depending on activity)_
- **Total Footprint**: ~25cm × 30cm _(estimated with legs extended)_

## CAD

All CAD files are designed in FreeCAD and can be found in the `CAD/` directory:

- **Corex2.0.FCStd** - Hip joint (coxa segment)
- **Femur2.0.FCStd** - Upper leg segment
- **Tibita2.1.FCStd** - Lower leg segment with foot
- **bodyhornsupport.FCStd** - Servo horn mounting bracket
- **extra part 2.0.FCStd** - Additional structural component
- **lowerrectangularbodyy.FCStd** - Lower body chassis panel
- **rectangularbodytop.FCStd** - Upper body chassis panel/cover

View the CAD designs with panels removed:

<img src="Images/Hexapod-CAD-Without-Cover.png" width="50%" alt="Hexapod Robot CAD without panels" />

## Assembly

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

## Credits

- Arduino community for microcontroller guidance.
- PCA9685 PWM board reference designs.
- Hexapod robotics open-source community for gait algorithms and kinematics.

## Thank you's

- Protoshred HQ team for design and assembly.
- FreeCAD community for excellent CAD tools.
- 3D printing community for printing tips and optimization.

## License

Hexapod Robot is open-source. More details can be found at [LICENSE.md](LICENSE.md).

![Hexapod Robot](Images/Hexapod-Assembled.jpg)
