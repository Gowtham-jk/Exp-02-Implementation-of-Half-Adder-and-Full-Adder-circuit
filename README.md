# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit
# Name : Gowtham . V
# REGISTER NUMBER : 23006362
# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
#### HALF ADDER:
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
#### FULL ADDER :
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
Logic symbol & Truthtable
RTL realization
### RTL
#### HALF ADDER:
![HALF ADDER](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/be4864e5-a131-4148-bdc9-eec82fe649bd)
#### FULL ADDER:
![FULL ADDER](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/7a966e29-3dbb-40d5-b95b-de2bd175f3f5)

### TRUTH TABLE :
#### HALF ADDER CIRCUIT:
![HALF ADDER TT](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/07881f8e-34b7-4bd3-9a11-eb3743539a4f)
#### FULL ADDER CIRCUIT:
![FULL ADDER TT](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/dccb327f-7c7a-4ef9-841e-19e55f9a5f91)



### OUTPUT:
#### HALF ADDER OUTPUT:
![HALF ADDER OUTPUT](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/650f4926-27a0-4970-be85-0b926b2d2dcc)
#### FULL ADDER OUTPUT:
![FULL ADDER OUTPUT](https://github.com/Gowtham-jk/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149857834/8fc9cd01-5e90-4933-8c6a-3a2251566e28)

### Result:
