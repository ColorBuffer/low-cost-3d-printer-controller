
The purpose of this project is to design an FDM 3d printer controller and keep the cost of that as lowest as possible.

# Motivation
As the most common homemade 3D printers are built with Arduino mega + a RAMP shield + 4 driver modules, the final price is too high.

We can make the cost lower by designing a unified board and remove its useless components.

# Solution

First, we should find a suitable microcontroller.

### 1) number of pins needed 

| used for                                 | count of pins |
|------------------------------------------|---------------|
| X-axis stepper controller                | 2             |
| Y-axis stepper controller                | 2             |
| Z-axis stepper controller                | 2             |
| extruder stepper controller              | 2             |
| all of XYZ endstops (sensors)            | 1             |
| WIFI communication                       | 2             |
| heated bed activation                    | 1             |
| heated bed thermistor                    | 1             |
| hotend thermistor                        | 1             |
| filament detector                        | 1             |
| SD card                                  | 4             |
| **total**                                | **19**        |