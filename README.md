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
- **Total Footprint**: ~45cm × 50cm _(estimated with legs extended)_

## BOM

Bill of materials and other notes can be found at [BOM.md](BOM.md).

## CAD

CAD files are designed in FreeCAD and stored in the `CAD/` directory:

- **CAD/Assemblies/** - Full assembly reference files (STEP format)
- **CAD/Parts/** - Individual 3D printable parts (STL format)
- **CAD/INVENTORY.md** - Component descriptions and assembly guide
- **CAD/BOM.md** - Detailed bill of materials

Full CAD file inventory can be found at [CAD/INVENTORY.md](CAD/INVENTORY.md).

View the CAD designs with panels removed:

<img src="Images/Hexapod-CAD-Without-Cover.png" width="50%" alt="Hexapod Robot CAD without panels" />

## Credits

- [Ruiqimao's Quicksilver](https://github.com/ruiqimao/Quicksilver/tree/main), for hexapod robotics inspiration.
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
