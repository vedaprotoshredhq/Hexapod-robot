# Hexapod Robot CAD Files

3D printing CAD files for the hexapod robot project. All STL files are optimized for FDM 3D printing.

## Directory Structure

- **Parts/** - Individual STL files ready for 3D printing
- **Assemblies/** - Full assembly files in STEP format (for reference and editing)

## 3D Printing Guide

### Recommended Print Settings
- **Layer Height:** 0.2mm
- **Infill:** 40%
- **Support Material:** Required everywhere
- **Print Speed:** 60mm/s for better quality
- **Nozzle Temperature:** 200-220°C (PLA) or 240°C (PETG)
- **Bed Temperature:** 60°C (PLA) or 80°C (PETG)

### Print Time & Material
Files larger than 2MB are stored with Git LFS for faster cloning and efficient storage.

## Software Required

| Purpose | Recommended Software |
|---------|---------------------|
| View STL | Any STL viewer, Cura, PrusaSlicer |
| View/Edit STEP | Fusion 360, FreeCAD (free), SolidWorks |
| Slice for Printing | Cura, PrusaSlicer, Ultimaker, Bambu Studio |

## File Types

- **STL files** - For 3D printing
- **STEP files** - Assembly reference and modifications

## Assembly Instructions

Refer to the main project README for assembly instructions on how to combine printed parts with electronics and mechanical components.

## Fasteners Required

- **2mm Screws** - For part assembly and securing components

## Notes

- Use appropriate adhesive/fasteners for assembly
