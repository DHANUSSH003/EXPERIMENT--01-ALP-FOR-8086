Name :Dhanussh Elango

Roll no: 212224040069

Date of experiment :29-8-25





## Aim: 
To Write and execute ALP on fundamental arithmetic and logical operations
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

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```


## Output  
 <img width="1920" height="1200" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/06f5573e-3f37-4623-b796-86decff45e33" />

## Subtraction   of 8 bit numbers  ALP 
```
 MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
<img width="1920" height="1200" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/f8a6b173-e06e-4644-b829-7e4a4658ae18" />

## Multiplication alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
 ## Output  

<img width="1920" height="1200" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/c6f0d6ae-1568-45e8-a869-c7d4984d0474" />

## Division alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  

<img width="1920" height="1200" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/63204ad4-13b1-4028-9e71-3ff58e958502" />

##Logical Operation:
##And:
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT
```
##OUTPUT:

<img width="1920" height="1200" alt="Screenshot (102)" src="https://github.com/user-attachments/assets/c382f452-64b6-4e70-9686-c1fb478ce9ca" />

##OR:
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT
```
##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (103)" src="https://github.com/user-attachments/assets/b098a6cf-dc4b-480e-b934-f3a3d110a470" />

##NOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (104)" src="https://github.com/user-attachments/assets/e4cf0989-2619-477c-bddb-7817b93f1369" />

##NAND:
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```

##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (105)" src="https://github.com/user-attachments/assets/3bcda287-8e53-40f3-b783-3fa5d74c0076" />

##NOT:
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT
```

##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (106)" src="https://github.com/user-attachments/assets/9529229e-9aa7-4735-9d8c-f3d46685f1b3" />

##XOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT
```
##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (107)" src="https://github.com/user-attachments/assets/cc1b69ad-d937-48f5-b6b0-1d75b21bd5e3" />

#XNOR:
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
##OUTPUT:
<img width="1920" height="1200" alt="Screenshot (108)" src="https://github.com/user-attachments/assets/cd79a484-5475-4978-94dc-5865e8a8384e" />

##TRUTH TABLE:

![WhatsApp Image 2025-08-29 at 10 48 39_d086650a](https://github.com/user-attachments/assets/a17d4dc7-329f-4f74-bd04-c755b1e00e59)


## Result :
Thus the program is verified and the desiered output is got
 








