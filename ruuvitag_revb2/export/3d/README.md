# 3D models of the PCB

## Procedudes how the models are created

### VRML
1) KiCad PCBnew -> File -> Export -> VRML

### STEP
1) Converted VRML file to STEP using [KiCad StepUp](http://sourceforge.net/projects/kicadstepup/)

## STL
1) Converted from STEP file using FreeCAD

## Bender
1) Open STL using Blender

### Convert STEP model to .wrl
[YouTube - Kicad StepUp tool: 3D Step and VRML File Alignment to footprint](https://youtu.be/O6vr8QFnYGw)

### Correct way to use StepUp
With kicad StepUp script, it is possible to work in kicad EDA with the same component model data available in the STEP AP214 3D format, and obtain a 3D STEP AP214 model of the pcb board and a complete board assemblies with electronic modules, to be used for MCAD interchange.
The accurate 3D visualization of components on board assemblies in kicad 3dviewer, can then be maintained in the same accuracy and aspect in STEP AP214 format, just generating VRML models from STEP or FreeCAD mechanical models and exporting the board through kicad StepUp script.
The kicad StepUp script maintains the usual way to work with kicad, but improves the process to work in a collaborative way with mechanical designers bringing near ECAD and MCAD environments.