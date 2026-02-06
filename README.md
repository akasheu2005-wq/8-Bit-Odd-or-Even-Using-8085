# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
```
LDA 4200H       
ANI 01H         
JZ EVEN 
JMP ODD
EVEN:
MVI A, 01H  
STA 4201H
HLT       
ODD: MVI A,02H
STA 4201H
HLT
```

## Output:

EVEN:
<img width="1898" height="915" alt="image" src="https://github.com/user-attachments/assets/5904d835-c1fb-44f9-ad2e-96767f442057" />

ODD:
<img width="1917" height="917" alt="image" src="https://github.com/user-attachments/assets/164fbf86-2a6f-4895-886a-180da3acdc6c" />

VERIFICATION:

![photo_2026-02-06_09-31-22](https://github.com/user-attachments/assets/2bf31cc0-3f89-44fb-a2ab-349f3865daa1)





## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

