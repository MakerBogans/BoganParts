# Roadkill Enhanced Toolhead PCB Family

The RKE family of toolhead boards are based off the roadkill board designed xbst_ but offer numerous improvements.

* Heater current capacity is greatly improved offering 5A of capacity on the RKE-Long board and 6A on RKE^2^. 
* Support for simultaneous use of neopixels, filament sensor, inductive probe and x endstop switch with dedicated ports for all features.
* All boards within the RKE family are pin compatible allowing for mix and matching of boards. 

## Important Notes

* Heater screw terminal is polarised, as the 24V supply is used as a common rail.
* Nylon or printed washers should be used to protect the mounting holes due to the proximity of the traces to the holes.
* LED port is designed for neopixels and uses a common 5V rail with the filament sensor port.
* Probe port has a 24V power rail.

## BOM

Per Board,

* 1 x 20 pin IDC header (2x10 2.54mm pitch)
* 5 x 2 pin JST-XH
* 3 x 3 pin JST-XH (2x for RKE Long)
* 1 x 4 pin JST-XH (2X for RKE Long)
* 1 x 5 mm pitch screw terminal (TB00250002BE)

## Pinout for Ports

IDC numbering is ODD_EVEN with 1 denoted by an arrow on the PCB

Pin 1 of the JST-XH ports is the square pads on the PCB.

For RKE^2^

| Port             | Pin 1 (IDC PIN)  | Pin 2  (IDC PIN) | Pin 3  (IDC PIN) | Pin 4 (IDC PIN) |
| ---------------- | ---------------- | ---------------- | ---------------- | --------------- |
| Layer Fan        | Fan Voltage (18) | Fan GND (20)     | -                | -               |
| Heater Fan       | Fan Voltage (14) | Fan GND (16)     | -                | -               |
| X endstop        | GND (2)          | Signal (12)      | -                | -               |
| Filament Sensor  | 5 V (4)          | GND (2)          | Signal (10)      | -               |
| Neopixel         | 5 V (4)          | GND (2)          | Data In (6)      | -               |
| Probe            | 24 (1,2)         | GND (2)          | Signal (8)       | -               |
| Thermistor (T0)  | T0 (11)          | GNDA (9)         | -                | -               |
| Extruder Stepper | A1 (19)          | A2 (17)          | B1 (15)          | B2 (13)         |
| Heater           | 24 V (1,3)       | HE GND (5,7)     | -                | -               |

RKE Long utilises a combined Filament Sensor and X endstop port pinout is below.

| Port                | Pin 1 (IDC PIN) | Pin 2  (IDC PIN) | Pin 3  (IDC PIN) | Pin 4 (IDC PIN) |
| ------------------- | --------------- | ---------------- | ---------------- | --------------- |
| Combined FS and XES | 5 V (4)         | GND (2)          | Signal (12)      | Signal (10)     |

