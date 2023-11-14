# Common Anode 7-Segment LED Display - Displaying Numbers 0-3

This repository contains code and wiring information to display numbers 0 to 3 on a Common Anode 7-segment LED display using an Arduino.

## Wiring

The display's segments (A-G) are connected to digital pins 2-8 on the Arduino, while the display's common anode is connected to digital pins 9-12.


### Pin Configuration

- `pinA` (2) - Segment A
- `pinB` (3) - Segment B
- `pinC` (4) - Segment C
- `pinD` (5) - Segment D
- `pinE` (6) - Segment E
- `pinF` (7) - Segment F
- `pinG` (8) - Segment G
- `D1` (9) - Common Anode Digit 1
- `D2` (10) - Common Anode Digit 2
- `D3` (11) - Common Anode Digit 3
- `D4` (12) - Common Anode Digit 4

## Code Explanation

The `setup()` function initializes the digital pins as outputs.

The `loop()` function sequentially displays numbers 0-3:
- `0`: All segments except G are turned on.
- `1`: Segments B and C are turned on.
- `2`: Segments A, B, D, E, and G are turned on.
- `3`: Segments A, B, C, D, and G are turned on.

Each digit is displayed for a brief duration of 1 millisecond, creating the appearance of sequential number display with a one-second interval.

Feel free to modify the code to display more numbers or alter the display timing as needed.

### Note

Ensure correct connections and use appropriate resistors for the LED segments to prevent damage to the components.

For further details, refer to the code comments and the provided wiring image.
