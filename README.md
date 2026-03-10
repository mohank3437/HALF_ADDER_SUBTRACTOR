HALF_ADDER_SUBTRACTOR
Implementation-of-Half-Adder-and-Half Subtractor-circuit

AIM:

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

<img width="449" height="225" alt="image" src="https://github.com/user-attachments/assets/f18d4f5d-c02e-4106-b937-f9b732f6c7b2" />


Figure -01 HALF ADDER

Half Subtractor

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B

<img width="524" height="298" alt="image" src="https://github.com/user-attachments/assets/fc8c1112-c9ed-4a03-b827-d66285217160" />


Figure -02 HALF Subtractor

Truthtable

<img width="247" height="150" alt="image" src="https://github.com/user-attachments/assets/ff839902-5e5f-40dc-ac41-ebfc7749167d" />

Procedure

Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

Program:
```
module Exp3(A,B,S1,C1,D1,B1);
input A,B;
output S1,C1,D1,B1;
assign S1=A^B;
assign C1=A&B;
assign D1=A^B;
assign B1=~A&B;
endmodule
```
Developed by:MOHAN K

RegisterNumber:212225240087

RTL Schematic

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5e4e6be2-c54f-4975-8075-b218e918407c" />


Output/TIMING Waveform

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/83d80629-86c6-4641-b459-359093721f0a" />



Result: Implementation-of-Half-Adder-and-Half Subtractor-circuit executed successfully.
