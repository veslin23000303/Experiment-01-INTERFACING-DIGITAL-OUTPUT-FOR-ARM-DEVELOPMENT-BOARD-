# Experiment-01-INTERFACING DIGITAL OUTPUT FOR ARM DEVELOPMENT BOARD 
## NAME : VESLIN ANISH A
## REG NO : 212223240175
## DATE : 10/03/2025

## Aim: To Interface a Digital output (LED) to ARM development board and write a blink code 
## Components required: STM32 CUBE IDE, NUCLEO ARM DEVELOPMENT BOARD  
## Theory 
The full form of an ARM is an advanced reduced instruction set computer (RISC) machine, and it is a 32-bit processor architecture expanded by ARM holdings. The applications of an ARM processor include several microcontrollers as well as processors. The architecture of an ARM processor was licensed by many corporations for designing ARM processor-based SoC products and CPUs. This allows the corporations to manufacture their products using ARM architecture. Likewise, all main semiconductor companies will make ARM-based SOCs such as Samsung, Atmel, TI etc.

What is an ARM7 Processor?
ARM7 processor is commonly used in embedded system applications. Also, it is a balance among classic as well as new-Cortex sequence. This processor is tremendous in finding the resources existing on the internet with excellence documentation offered by NXP Semiconductors. It suits completely for an apprentice to obtain in detail hardware & software design implementation.
LPC2148 Microcontroller
 The LPC2148 microcontroller is designed by Philips (NXP Semiconductor) with several in-built features & peripherals. Due to these reasons, it will make more reliable as well as the efficient option for an application developer. LPC2148 is a 16-bit or 32-bit microcontroller based on ARM7 family.
Features of LPC2148
The main features of LPC2148 include the following.
•	The LPC2148 is a 16 bit or 32 bit ARM7 family based microcontroller and available in a small LQFP64 package.
•	ISP (in system programming) or IAP (in application programming) using on-chip boot loader software.
•	On-chip static RAM is 8 kB-40 kB, on-chip flash memory is 32 kB-512 kB, the wide interface is 128 bit, or accelerator allows 60 MHz high-speed operation.
•	It takes 400 milliseconds time for erasing the data in full chip and 1 millisecond time for 256 bytes of programming.
•	Embedded Trace interfaces and Embedded ICE RT offers real-time debugging with high-speed tracing of instruction execution and on-chip Real Monitor software.
•	It has 2 kB of endpoint RAM and USB 2.0 full speed device controller. Furthermore, this microcontroller offers 8kB on-chip RAM nearby to USB with DMA.
•	One or two 10-bit ADCs offer 6 or 14 analogs i/ps with low conversion time as 2.44 μs/ channel.
•	Only 10 bit DAC offers changeable analog o/p.
•	External event counter/32 bit timers-2, PWM unit, & watchdog.
•	Low power RTC (real time clock) & 32 kHz clock input.
•	Several serial interfaces like two 16C550 UARTs, two I2C-buses with 400 kbit/s speed.
•	5 volts tolerant quick general purpose Input/output pins in a small LQFP64 package.
•	Outside interrupt pins-21.
•	60 MHz of utmost CPU CLK-clock obtainable from the programmable-on-chip phase locked loop by resolving time is 100 μs.
•	The incorporated oscillator on the chip will work by an exterior crystal that ranges from 1 MHz-25 MHz
•	The modes for power-conserving mainly comprise idle & power down.
•	For extra power optimization, there are individual enable or disable of peripheral functions and peripheral CLK scaling.
 
 

## Procedure:
 1. click on STM 32 CUBE IDE, the following screen will appear 
 ![image](https://user-images.githubusercontent.com/36288975/226189166-ac10578c-c059-40e7-8b80-9f84f64bf088.png)

 2. click on FILE, click on new stm 32 project 
 ![image](https://user-images.githubusercontent.com/36288975/226189215-2d13ebfb-507f-44fc-b772-02232e97c0e3.png)
![image](https://user-images.githubusercontent.com/36288975/226189230-bf2d90dd-9695-4aaf-b2a6-6d66454e81fc.png)
3. select the target to be programmed  as shown below and click on next 

![image](https://user-images.githubusercontent.com/36288975/226189280-ed5dcf1d-dd8d-43ae-815d-491085f4863b.png)

4.select the program name 
![image](https://user-images.githubusercontent.com/36288975/226189316-09832a30-4d1a-4d4f-b8ad-2dc28f137711.png)


5. corresponding ioc file will be generated automatically 
![image](https://user-images.githubusercontent.com/36288975/226189378-3abbdee2-0df6-470f-a3cd-79c74e3d3ad8.png)

6.select the appropriate pins as gipo, in or out, USART or required options and configure 
![image](https://user-images.githubusercontent.com/36288975/226189403-f7179f1a-3eae-4637-826b-ab4ec35ba1e1.png)
![image](https://user-images.githubusercontent.com/36288975/226189425-2b2414ce-49b3-4b61-a260-c658cb2e4152.png)


7.click on cntrl+S , automaticall C program will be generated 
![image](https://user-images.githubusercontent.com/36288975/226189443-8b43451d-0b14-47e4-a20b-cc09c6ad8458.png)
![image](https://user-images.githubusercontent.com/36288975/226189450-85ffa969-2ffb-4788-81e5-72d60fdda0f1.png)
8. edit the program and as per required 
![image](https://user-images.githubusercontent.com/36288975/226189461-a573e62f-a109-4631-a250-a20925758fe0.png)

9. use project and build all 
![image](https://user-images.githubusercontent.com/36288975/226189554-3f7101ac-3f41-48fc-abc7-480bd6218dec.png)
10. once the project is bulild link the hexfile build in stm32cube ide using post processor build 
![image](https://user-images.githubusercontent.com/36288975/226189577-c61cc1eb-3990-4968-8aa6-aefffc766b70.png)

11. click on debug option 
![image](https://user-images.githubusercontent.com/36288975/226189625-37daa9a3-62e9-42b5-a5ce-2ac63345905b.png)


12. connect the stm nucleo board and click on run 
![image](https://user-images.githubusercontent.com/36288975/226189649-b5dff389-91df-4eca-b84a-1127c6562637.png)






## STM 32 CUBE PROGRAM :
## ADDITION OF 8 BIT ALP:
```
MOV AL,74H
MOV BL,69H
ADD AL,BL
HLT
```
## OUTPUT:
![Screenshot 2025-02-28 083119](https://github.com/user-attachments/assets/3d4f0f07-fb87-4e32-bb8d-c3d5d2dbace3)

## SUBTRACTION OF 8 BIT ALP:
```
MOV AL,74H
MOV BL,69H
SUB AL,BL
HLT
```
## OUTPUT:
![Screenshot 2025-02-28 083443](https://github.com/user-attachments/assets/59fb8c36-1920-4378-9611-083d2f1f4f08)

## MULTIPLICATION OF 8 BIT ALP:
```
org 100h
MOV AL,75H
MOV BL,32H
MUL BL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 084501](https://github.com/user-attachments/assets/47c0e819-6ca6-4ca0-96fa-a67fbc489dc0)

## DIVISION OF 8 BIT ALP:
```
org 100h
MOV AL,70H
MOV BL,10H
DIV BL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 085310](https://github.com/user-attachments/assets/9d192f60-580f-4e2e-b364-a9a5ea16c975)

## AND GATE OF 8 BIT ALP:
```
org 100h
MOV AL,33H
MOV BL,44H
AND AL,BL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 085449](https://github.com/user-attachments/assets/2102ce1d-68f8-4a62-bf5b-0d8854dc211a)


## OR GATE OF 8 BIT ALP:
```
org 100h
MOV AL,33H
MOV BL,44H
OR AL,BL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 085953](https://github.com/user-attachments/assets/a83f45b0-01dc-4de5-b4d0-01f8b4b59371)


## NOT GATE OF 8 BIT ALP:
```
org 100h
MOV AL,65H
NOT AL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 090356](https://github.com/user-attachments/assets/042fe44d-6ba6-4cd3-ad1b-fc038502d2ec)


## XOR GATE OF 8 BIT ALP:
```
org 100h
MOV AL,66H
MOV BL,77H
XOR AL,BL
HLT
ret
```
## OUTPUT:
![Screenshot 2025-02-28 091023](https://github.com/user-attachments/assets/e4d10e74-fa8b-49bf-ae28-2a96952ce952)

## Result :
Interfacing a digital output with ARM microcontroller is executed and the results are verified.


