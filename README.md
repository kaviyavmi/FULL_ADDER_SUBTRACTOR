# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**TRUTH TABLE**

FULL ADDER

![WhatsApp Image 2024-12-21 at 09 58 44_a02f2549](https://github.com/user-attachments/assets/6b043e95-fb65-4f95-8fff-b687847cc3f1)

FULL SUBRACTOR

![WhatsApp Image 2024-12-21 at 09 59 03_094b7638](https://github.com/user-attachments/assets/80fc4c77-fad1-41bd-8de2-c6bb78c23c92)



**Procedure**


1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

i)FULL ADDER

module fa(a,b,cin,sum,carry);

input a,b,cin;

output sum,carry;

assign sum=( (a ^ b)^cin);

assign carry= ( (a & b)| ( cin &(a ^ b )));

endmodule

ii)FULL SUBTRACTOR

module fs(a,b,bin,difference,borrow);

input a,b,bin;

output difference,borrow;

assign difference= ((a ^ b)^bin);

assign borrow= ((~a & b)|(bin & (~(a ^ b))));

endmodule

Developed by:Kaviya.V.M

RegisterNumber:24900714



**RTL Schematic**

FULL ADDER RTL

![Full adder sum](https://github.com/user-attachments/assets/4d2c37db-79fc-490a-8b22-b09edf779b89)

FULL SUBRACTOR RTL

![full subtractor ](https://github.com/user-attachments/assets/5fbf92cd-3c16-4909-a868-7c8d696c281c)


**Output**

FULL ADDER WAVEFORM

![Full adder sum waveform](https://github.com/user-attachments/assets/05c54a2c-29d2-4a34-9a1f-1441f41de5e4)

FULL SUBRACTOR WAVEFORM

![full subtractor waveform](https://github.com/user-attachments/assets/4adddc62-bfd0-48d6-8009-d4a22ff1b26c)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



