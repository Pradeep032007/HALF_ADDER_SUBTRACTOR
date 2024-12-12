### NAME :PRADEEP B
### REGISTER NO :24900484
### EXPERIMENT 3: HALF ADDER SUBRACTOR
### AIM
To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

### EQUIPEMENT REQUIRED
Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

### HALF ADDER
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![WhatsApp Image 2024-12-12 at 13 45 52_5d1052ad](https://github.com/user-attachments/assets/3bd210d1-1105-4362-a2f7-12fdc6cb3cb6)


Figure -01 HALF ADDER

### HALF SUBRACTOR
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.

Diff = A’B+AB’ =A ⊕ B Borrow = A’B
![WhatsApp Image 2024-12-12 at 13 46 28_90ec31d7](https://github.com/user-attachments/assets/99a2f49f-60b0-4ccf-bcc2-647491a3a7d6)



Figure -02 HALF Subtractor

### TRUTH TABLE
![WhatsApp Image 2024-12-12 at 13 46 21_b5d6bb0a](https://github.com/user-attachments/assets/4c34bb1c-6466-4625-b6be-855724fec102)


### PROCEDURE
Type the program in Quartus software.

Compile and run the program.

Generate the RTL schematic and save the logic diagram.

Create nodes for inputs and outputs to generate the timing diagram.

For different input combinations generate the timing diagram.

### PROGRAM
# module halfaddsub(a,b,sum,carry,difference,borrow);
# input a,b;
# output sum,carry,difference,borrow;
# assign sum=a^b;
# assign carry=a&b;
# assign difference=a^b;
# assign borrow=(~a)&b;
# endmodule

### RTL OUTPUT
![WhatsApp Image 2024-12-12 at 13 46 26_95084175](https://github.com/user-attachments/assets/7a008819-53cd-4028-8bee-ef163b5f04ec)


### OUTPUT WAVEFORM
![WhatsApp Image 2024-12-12 at 13 46 25_ef0c57e3](https://github.com/user-attachments/assets/b45faa84-740e-41d5-829b-a33911f69145)


### RESULT
Thus design a half adder and half subtractor circuit and verified its truth table in Quartus using Verilog programming
