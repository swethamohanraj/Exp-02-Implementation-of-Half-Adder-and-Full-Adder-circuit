# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
```*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:K.M.SWETHA
RegisterNumber: 212221240055

HALF ADDER

module Adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

FULL ADDER

module FullAdder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
*/
```

### Output:
## Half Adder:
### Logic Symbol
![image](https://user-images.githubusercontent.com/94228215/165551860-c674a011-695f-4813-a026-10c47acbdb91.png)

### RTL
![image](https://user-images.githubusercontent.com/94228215/165551922-31c2d38e-8674-4b07-8b2a-68771b6dd16f.png)



### TIMING DIAGRAM
![timimgdia](https://user-images.githubusercontent.com/94228215/166901030-18277d00-1bd3-4858-8e60-06acf0c8646d.jpeg)




### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/94228215/165551985-b0b4faae-f7da-4c2f-9dde-d320766088c7.png)

## Full Adder:
### Logic Symbol
![image](https://user-images.githubusercontent.com/94228215/165554067-9cf49122-9d0a-41bc-bf9d-b7cec9fe9cc7.png)


### RTL Realization
![image](https://user-images.githubusercontent.com/94228215/165554141-2d5fbd37-5687-4867-8d17-46ef49c2ee73.png)


### Truthtable
![image](https://user-images.githubusercontent.com/94228215/165554199-60547f18-7a93-4eb8-8358-ca3d34b59824.png)


### Timing Diagram
![image](https://user-images.githubusercontent.com/94228215/165554238-cdb76294-e878-4135-9100-b54d458610cf.png)



### Result:
Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
