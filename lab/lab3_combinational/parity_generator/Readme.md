# Parity generator

Using Board Basys3 with 10ns clock period.

## Design

This design is to generate the parity bit of the input binary number.

* The data binary_in is the input binary number.
* The data parity is the output parity bit.

The vivado design is based on the diagram shown below:

**Note that during Vivado compilation of the for-loop, the design will be implemented with a balanced structure instead of a skewed one.**
![Alt text](image-4.png)

## Result comparison

|Waveform||
|--|--|
|HLS|![Alt text](image.png)|
|verilog|![Alt text](image-2.png)|

The screenshot only displays a portion of the results. Nonetheless, the correctness of both designs has been verified through simulation.

|Utilization||
|--|--|
|HLS|![Alt text](image-1.png)|
|verilog|![Alt text](image-3.png)|

The reports indicate that the utilization is the same in both the HLS-designed and Verilog-designed implementations.