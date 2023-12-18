# Name: Prajin S
# Register Number: 23012918

# Exp 02 Implementation of Half Adder and Full Adder circuit

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
#### Figure -01 HALF ADDER 
![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)
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
![Screenshot 2023-12-18 122856](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/92e73879-5924-402f-9e6b-783024e0b164)

### RTL Realization
![Screenshot 2023-12-18 104731](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/78229cd7-b021-4f9a-b42e-03bcb4c3b328)

### Timing Diagram
![Screenshot 2023-12-18 104912](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/91cb00a2-6ca0-4907-9cb8-2c5e973ffb00)

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

#### Figure -02 FULL ADDER 
![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)
 
### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

### Truth Table
![Screenshot 2023-12-18 123750](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/c9fd9c60-3486-480b-890e-62f8a2dd25b0)

### RTL realization
![Screenshot 2023-12-18 110210](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/05f85db2-6018-460a-a695-71bf8ed54fe2)

### Timing Diagram
![Screenshot 2023-12-18 110556](https://github.com/vasanthkumarch/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/144979377/7f8bb17d-4701-4a97-88c5-b11935075b27)


### Result:
Thus,half adder and full adder are studied and truth tables for different logic gates are verified.
