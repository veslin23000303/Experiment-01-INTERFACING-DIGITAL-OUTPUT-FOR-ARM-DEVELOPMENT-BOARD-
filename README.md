## EXPERIMENT--01-ALP-FOR-8086
## Name : VESLIN ANISH A

## Roll no : 212223240175

## Date of experiment : 21.8.2024

## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086 emulator
## Theory
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.

## Running the Emulator :
1.Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory

2.Run emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color

 3.write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 
 
4.Compile the program and check for the errors

5.Run (once there is no syntax error)

6.Click OK to see/view the output of your program on the Emulator screen.

7.After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,

8.
![189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04](https://github.com/user-attachments/assets/bace2e68-d36b-4e6c-8e49-35c6900e9f81)



9.Click on emulate to start emulation

![189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc](https://github.com/user-attachments/assets/ad7d228a-0e3a-4039-890c-cfbc629990cf)


10.If no errors are found click on run the program and check the status of various flags in the flags tab as shown below

![189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe](https://github.com/user-attachments/assets/7c16fb74-8cfa-4593-aa85-c5330e3fab71)


## Programs for arithmetic operations
## Addition of 8 bit ALP
```
org 100h
MOV al,11h;
MOV bl,20h;
ADD al,bl;
MOV [6379h],al;
ret
```
## Output:
![359149943-115a2ddb-c4f1-4479-a940-fc1784f5deb2](https://github.com/user-attachments/assets/00784ea7-8c10-4300-b63a-5d835f5ceb29)


## Subtraction of 8 bit numbers ALP:
```
org 100h
MOV al,20h;
MOV bl,[8778h];
SUB bl,al;
MOV [8798h],bl;
ret
```
## output:
![Screenshot 2024-08-21 142725](https://github.com/user-attachments/assets/de1c079d-1052-41da-a9a0-cc0407535542)

## Multiplication alp:
```
org 100h
 MOV al,13h;
 MOV bl,2h;
 MUL bl;
 MOV [6063h],bl;
 ret
```
## Output:
![Screenshot 2024-08-21 143059](https://github.com/user-attachments/assets/bafebcc4-180b-44ec-b20d-c9e46206398d)

## Division alp:

```
org 100h
 MOV al,26h;
 MOV bl,[2369h];
 DIV bl;
 MOV [2399h],al;
 ret
```
## output:
![Screenshot 2024-08-21 224750](https://github.com/user-attachments/assets/1db56b2b-00b7-4217-a998-a1e292ecf6fb)

## Programs For Logical Operators:
## AND
```
org 100h
mov bx,1000h;
and bx,1111h;
mov [0040h+02],bx;
ret
```
## output:
![Screenshot 2024-08-21 222956](https://github.com/user-attachments/assets/c2b51b12-462b-4109-9286-0216c92aa912)

## or:
```
MOV SI,0532H;
MOV AX,0A32H;
MOV BX,0B13H;
OR AX,BX;
```
## output:

![Screenshot 2024-08-21 223433](https://github.com/user-attachments/assets/af11a859-2d0c-405a-9735-07198e672b81)

## NOT:
```
org 100h
mov bx,0040h;
mov ax,[bx]; 
not al;
mov [0040h+04],ax;
ret
```
## output:
![359154412-80e5a7d3-89b9-4756-ae19-8ab5fa6844f6](https://github.com/user-attachments/assets/931ee947-a992-4560-af16-7388ce237934)

## XOR:
```
MOV [SI+2],AX;
MOV AX,0A32H;
MOV BX,0B13H;
XOR AX,BX;
```
## output:
![359155181-f90ba85a-5455-4f20-b4bc-2ad80fcbd183](https://github.com/user-attachments/assets/847d7c1d-694a-4014-8c52-91594143c0b3)
## Result:Thus, to write and execute ALP on fundamental arithmetic operations and Logical operations is successful.

