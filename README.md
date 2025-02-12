# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
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

### 

Program:

/*

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: P.Jeba Princy

RegisterNumber: 22008375

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
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: P.Jeba Princy
RegisterNumber: 22008375
*/
HALF ADDER
module halfadder(A,B,Sum,Carry);
input A,B;
output Sum,Carry;
xor(Sum,A,B);
and(Carry,A,B);
endmodule

FULL ADDER
module fulladder(A,B,C,Sum,Carry);
input A,B,C;
output Sum,Carry;
assign Sum =((A^B)^C);
assign Carry = ((A&B)|(B&C)|(C&A));
endmodule
Logic symbol & Truthtable
RTL realization
![HALF ADDER](https://user-images.githubusercontent.com/122682918/213922376-c9e4159c-b504-4033-9962-b793bcd02005.png)

### Output:
### RTL
![Screenshot (4)](https://user-images.githubusercontent.com/122682918/213922421-29b115c3-10e0-41ff-ba06-90b7656a1fd7.png)



### TIMING DIGRAM
![image](https://user-images.githubusercontent.com/122682918/213923562-dd158b89-b596-41b1-ae75-adc4369d4737.png)![image](https://user-images.githubusercontent.com/122682918/213924971-a05e145d-acd9-49d1-97bf-3d6c76454b5e.png)










### TRUTH TABLE
The Truth Table For Half Adder
![image](https://user-images.githubusercontent.com/122682918/213925044-6e1225f8-d2d0-422c-94c6-c4f479d01714.png)

The Truth Table For Full Adder
![image](https://user-images.githubusercontent.com/122682918/213925093-c612c902-5782-46e7-afda-cdabbc29c1ef.png)



### Result:
Thus the half adder and full adder circuit was successfully implemented
