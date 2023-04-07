# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit

# AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

# Equipments Required:

Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

# Half Adder:

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

# Full Adder:
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

# Figure -01 HALF ADDER :


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

# Figure -02 FULL ADDER :

# Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

# Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: NIROSHA.S 
RegisterNumber: 212222230097

# Half adder program:

module Halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

# Full adder program:

module Fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum =((a^b)^c);
assign carry =((a&b)|(b&c)|(c&a));
endmodule
*/

# Logic symbol & Truthtable:

# HALF ADDER:

![DE ha3](https://user-images.githubusercontent.com/121418437/230565259-90ee0d0d-dbb0-4d10-b982-6d61042e3086.png)

# FULL ADDER:
![DE fa3](https://user-images.githubusercontent.com/121418437/230565306-79b848e8-f3f1-4398-b19f-ddd1b17cc2e2.png)

### Output:

# RTL realization:

# HALF ADDER:

![DE ha1](https://user-images.githubusercontent.com/121418437/230565692-104e435c-708a-4ff2-8206-1e0f6e786abd.PNG)

# FULL ADDER:

![DE fa1](https://user-images.githubusercontent.com/121418437/230565760-64fc6fc2-cd06-46c3-8047-43ce06d6b2ff.PNG)

### TIMING DIAGRAM:

# HALF ADDER:

![DE ha2](https://user-images.githubusercontent.com/121418437/230566053-33fc1d86-40bb-4126-b46e-130cb202ee71.PNG)

# FULL ADDER:

![DE fa2](https://user-images.githubusercontent.com/121418437/230566083-7b89435c-b839-4e55-9398-860090ef6250.PNG)

# TRUTH TABLE :

# HALF ADDER:

![DE ha4](https://user-images.githubusercontent.com/121418437/230566184-c05edc5c-028d-4410-a22d-32b32353f8dc.png)

# FULL ADDER:

![DE fa4](https://user-images.githubusercontent.com/121418437/230566220-8f1ae3db-5937-4e0b-9110-8b7824a8e924.png)

# Result:
    Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
