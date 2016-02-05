## [KiCad StepUp](http://sourceforge.net/projects/kicadstepup/)to create AP214 STEP file

## Prerequisities
* IDFv3 export (.emp) from PCBnew (KiCad >4.0)
* [FreeCAD](http://www.freecadweb.org/) >0.15
* Every .wrl 3D model should have corresponding .step file (we don't, yet)

## How to use
1) Export IDFv3
2) Run the script from Terminal:
`/Applications/FreeCAD.app/Contents/MacOS/freecad ../ruuvitag_revb2/ruuvitag_revb2.emn ksu-config.cfg kicad_StepUp.FCMacro`
3) .step will be created automatically. Done.

## TODO
* Create new 3d Models (STEP and VRML). Best way is to export VRML model from STEP using FreeCAD: [YouTube - Kicad StepUp tool: 3D Step and VRML File Alignment to footprint](https://youtu.be/O6vr8QFnYGw).