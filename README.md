# Experiment--03-Half-Subtractor-and-Full-subtractor
## Implementation-of-Half-subtractor-and-Full-subtractor-circuit
## AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
## Theory
Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

## Half Subtractor Full Subtractor
## Half Subtractor
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed.
![half-subtractor9](https://user-images.githubusercontent.com/36288975/166112538-58c3bc7c-ee5d-4e6a-ac8d-8e8328efe27a.png)


Sum = X'Y+XY' = X ⊕ Y
Carry=X'Y

## Full Subtractor
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. 
![full-subtractor6](https://user-images.githubusercontent.com/36288975/166112541-24c68359-3de8-4674-ae22-8272ffc385ed.png)


Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

## Procedure



Write the detailed procedure here 


## Program:
/*
Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
Developed by: Revanth Palagiri

RegisterNumber:  23002622

program:
![ Image 2024-01-02 at 21 44 17_ed2e7fdb](https://github.com/Revanth-2717/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/152462274/e5bdcbd4-d736-48e2-a44b-01e067398d02)

## Output:

## Truthtable
![Image 2024-01-02 at 21 50 35_c35f9748](https://github.com/Revanth-2717/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/152462274/883057fb-5d94-4911-8570-c5bfcef8e43a)
![Image 2024-01-02 at 21 51 29_6e5c617e](https://github.com/Revanth-2717/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/152462274/07382305-a0b1-497c-9be7-c04efc00cf00)


##  RTL realization:
![ Image 2024-01-02 at 21 45 19_db729578](https://github.com/Revanth-2717/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/152462274/7f390e07-ea24-418d-bab5-b1eebac79950)

## Timing diagram: 
![ Image 2024-01-02 at 21 49 32_f25f5908](https://github.com/Revanth-2717/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/152462274/65b00ccf-1df2-4d3e-812c-11b13aa4c797)

## Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
