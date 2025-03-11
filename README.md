# EXPERIMENT--01-ALP-FOR-8086
```
Name :VINODINI R
Roll no :212223040244
Date of experiment :11-03-2025
```




## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition,Subtraction,Multiplication,Division  of 2byte ALP
```
org 100h 
MOV AX,1122H
MOV BX,2233H
ADD AX,BX 
MOV [6000H],AX
     
     ;DIRECT ADDR MODE
MOV AX,[5000H]
MOV BX,[5002H]  ;2 BYTE ADDR
MOV AX,BX
MOV [6010H],AX

;REGISTER ADDR MODE  
MOV BX,4444H
MOV AX,BX
MOV CX,3333H
MOV DX,CX
MUL DX
MOV [6020H],AX

;INDIRECT ADDR MODE   
MOV BX,5005H
MOV AX,[BX] 
MOV CX,01H
DIV CX      
MOV [6030H],AX
ret
```
## Output  

![Screenshot 2025-03-11 104319](https://github.com/user-attachments/assets/d77d5120-dd43-4fc9-92b0-1056f8e968f7)

## Logical AND
```
org 100h
MOV AL,33H
MOV BL,44H
AND AL,BL
ret
```
## OUTPUT

![Screenshot 2025-03-11 110452](https://github.com/user-attachments/assets/f7538ce5-2549-4c89-89a1-1005136335d4)

## Logical OR

```
org 100h
MOV AL,45H
MOV BL,66H
OR AL,BL
ret
```

## OUTPUT

![Screenshot 2025-03-11 110741](https://github.com/user-attachments/assets/7611c6d2-4bee-4cdb-9b1c-952da512cac9)

## Logical NOT

```
org 100h
MOV AL,65H
NOT AL
ret
```
## OUTPUT

![Screenshot 2025-03-11 111106](https://github.com/user-attachments/assets/72f9d94c-e782-4667-8eed-3c543e9bbb8e)

## Logical XOR

```
org 100h
MOV AL,66H
MOV BL,77H
XOR AL,BL
ret
```
## OUTPUT

![Screenshot 2025-03-11 111507](https://github.com/user-attachments/assets/52aa1b73-fc0a-4493-ab5c-5e71e912fcd3)


## Result :
The execution of ALP on fundamental arithmetic and logical operations is successfully completed.
