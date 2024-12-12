### NAME :PRADEEP.B
### REGISTER NO :24900484
# EXPERIMENT 3: HALF ADDER SUBRACTOR
AIM
To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

EQUIPEMENT REQUIRED
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

HALF ADDER
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

image

Figure -01 HALF ADDER

HALF SUBRACTOR
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B

image

Figure -02 HALF Subtractor

TRUTH TABLE
image

PROCEDURE
Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

PROGRAM
module halfaddsub(a,b,sum,carry,difference,borrow); input a,b; output sum,carry,difference,borrow; assign sum=a^b; assign carry=a&b; assign difference=a^b; assign borrow=(~a)&b; endmodule

RTL OUTPUT
image

OUTPUT WAVEFORM
image

RESULT
Thus design a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming
