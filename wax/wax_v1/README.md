# Wax V1
Wax V1 is a passive multiple module (V2 for buffered mults comming?). It functions as a 1x6 or 2x3 multiple, with the inputs normalised together.

## Operation
- The 2 inputs are marked with the solid polys. They are normalised together, meaning if a single input is used, the signal will be propagated to all 6 outputs.
- The outputs are marked with the hollow polys.
- The passive nature of `Wax V1` means that it is best used for triggers/gates and CV signals where accurate voltage tracking is not required.
- For driving several oscillators, where accurate 1v/Oct tracking is important, it would be best to use a buffered mult.

## Repo Overview
- `wax_v1_FP` : KiCAD project files for the module front panel
- `wax_v1_FP_gerber` : fabrication files for the front panel PCB (JLCPCB spec)
- `wax_v1_FP_graphics` : SVG graphics used in the development of the front panel PCB
- `wax_v1_PCB` : KICAD project files for the main PCB
- `wax_v1_PCB_gerber` : fabrication files for the main PCB (JLCPCB spec)

## Build Notes
- The main PCB can be manufactured as a 2 layer PCB, using default settings on JLCPCB
- The front panel can also use mostly default settings too.
	+ It was designed with black solder resist in mind
	+ ENIG surface finish may give the best results/longevity of the metal designs
- Ground pads are shared between pairs of jack sockets
- Knurled nuts are probably the best option aesthetically
	+ I didn't consider the radius of the nut when designing the front panel graphics
	+ Befaco knurled nuts look good, in a combination of black and yellow, but there may be some overlap of the graphics due to the larger diameter when compared to a standard knurled nut

## BOM
| Part | Qty |
|------|-----|
|wax_v1_PCB|1|
|wax_v1_FP |1|
|Thonkiconn mono jack|8|
|Knurled m6 nut|8|