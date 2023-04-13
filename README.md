# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
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

## Procedure:

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
## Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Laakshit D
RegisterNumber:212222230071

HALF ADDER:
module halfadder(A,B,C,S);
input A,B;
output S,C;
xor(S,A,B);
and(C,A,B);
endmodule

FULL ADDER:
module fulladd(a,b,ci,s,co);
input a,b,ci;
output s,co;
wire d,e,f;
xor(d,a,b);
xor(s,d,ci);
and(e,ci,d);
and(f,a,b);
or(co,e,f);
endmodule  
*/
```
Logic symbol & Truthtable
RTL realization

## Output:
### RTL
### HALF ADDER
![out1](https://user-images.githubusercontent.com/119559976/231803741-ac581b0d-35ca-4ed8-9006-451e363e2e97.png)

### FULL ADDER
![out2](https://user-images.githubusercontent.com/119559976/231803790-eb0baa79-f670-46d3-80ad-dbf73d9e4b96.png)

## TIMING DIAGRAM:
### HALF ADDER
![td1](https://user-images.githubusercontent.com/119559976/231803837-eca7da10-d3ae-4a53-85c4-2828bfcf41c7.png)
### FULL ADDER
![td2](https://user-images.githubusercontent.com/119559976/231803868-d627aee3-26f8-4e02-b77a-50df242959d5.png)

## TRUTH TABLE:
### HALF ADDER
![ttout1](https://user-images.githubusercontent.com/119559976/231803913-d65ddf6f-62aa-4f39-a8b3-065f095a3cf1.png)
### FULL ADDER
![ttout2](https://user-images.githubusercontent.com/119559976/231803955-54e605de-d790-45ef-8313-474e9e300f03.png)

## Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
