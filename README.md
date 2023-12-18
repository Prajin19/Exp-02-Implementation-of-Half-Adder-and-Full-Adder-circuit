# Name:Prajin S
# Register Number:23012918
# Exp 02:Implementation of Half Adder and Full Adder circuit

# Implementation of Half Adder and Full Adder circuit
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


 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 
### Program:
```
module Halfadder (a,b,sum,carry);
input a,b;
output sum,carry;
xor (sum,a,b);
and (carry,a,b);
endmodule
```
### Truth Table
![Screenshot 2023-12-18 122856](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/c91b8656-69c0-4a04-a7ff-ba388c45ccc5)
### RTL Realization
![Screenshot 2023-12-13 173413](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/5854aa93-2856-4531-96b3-834180bceecd)
### Timing Diagram
![Screenshot 2023-12-18 104912](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/d547d99a-34ca-4ade-94ea-64cefd1a02bb)

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### Program:
```
module Fulladder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b|c& a^ c&b ;
endmodule
```
### Truth Table 
![Screenshot 2023-12-18 123750](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/d5e398a2-7999-4dc6-92bf-17841663084d)
### RTL Realization
![Screenshot 2023-12-18 110210](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/80b59a8a-0bfe-4a76-904a-972722910e74)
### Timing Diagram
![Screenshot 2023-12-18 110556](https://github.com/Prajin19/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/250adc12-2da9-48d6-82fe-6e95d59e453b)

### Result:
Thus,half adder and full adder are studied and the truth table for different logic gates are verified.
