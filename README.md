# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: MUGIL RAJ S A 
RegisterNumber: 212223220062

HALF ADDER 

```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = a^b;
assign carry = a&b;
endmodule

```
HALF SUBTRACTOR

```
module halfsubt(a,b,diff,Bo);
input a,b;
output diff,Bo;
assign diff = a^b;
assign bo = ~a & b;
endmodule

```
**RTL Schematic**

HALF ADDER

![Screenshot 2024-10-10 105409](https://github.com/user-attachments/assets/f48f1776-8134-4189-9840-36349fc500c3)

HALF SUBTRACTOR 

![Screenshot 2024-10-10 111111](https://github.com/user-attachments/assets/aea45f72-5691-4696-a732-a98ab99764ad)


**Output/TIMING Waveform**

HALF ADDER

![Screenshot 2024-10-10 110244](https://github.com/user-attachments/assets/385b859c-fff3-4ff9-b2b7-b5670e8099eb)


HALF SUBTRACTOR 

![Screenshot 2024-10-10 111707](https://github.com/user-attachments/assets/bd1966cf-aeaa-4afa-b4e7-928cb438935f)

**Result:**

Thus, the given half adder and half subracter executed successfully using quartus.
