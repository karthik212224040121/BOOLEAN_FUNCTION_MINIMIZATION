# BOOLEAN_FUNCTION_MINIMIZATION

*AIM:*

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

*Equipment Required:*

Hardware – PCs, Cyclone II , USB flasher

*Software – Quartus prime*

*Theory*
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

*Boolean Expression*
(i)F1
![WhatsApp Image 2024-12-21 at 11 58 25_9688a08b](https://github.com/user-attachments/assets/2127cbcc-68f8-43a9-9836-bcb6ae081551)

(ii)F2
![WhatsApp Image 2024-12-21 at 11 58 44_e0a93405](https://github.com/user-attachments/assets/d7010a77-ceb2-4ff1-bb61-2088ed53eb78)
*Truth Table*


(i)F1

![Screenshot 2024-12-24 112423](https://github.com/user-attachments/assets/bb6c21cc-aa3f-4693-82cc-92d656e48af8)

(ii)F2

![Screenshot 2024-12-24 112428](https://github.com/user-attachments/assets/9c30c5aa-a560-4676-bc25-60d49d6314cd)

*Procedure*

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


*Program:*

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: pothu sumanth
RegisterNumber: 24000831

        i)F1
        module funct1(a,b,c,d,f1);
        input a,b,c,d;
        output f1;
        assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
        endmodule

      ii)F2
      module funct2(w,x,y,z,f2);
      input w,x,y,z;
      output f2;
      assign f2=((~y & z)|( w & y )|(x & y));
      endmodule



*RTL realization*


(i)F1


![WhatsApp Image 2024-12-24 at 11 31 06_e34debe5](https://github.com/user-attachments/assets/adb50b8e-45b1-4029-8137-fa601f0a86ab)

(ii)F2

![Screenshot 2024-12-27 135405](https://github.com/user-attachments/assets/8c882460-a61e-4acb-b6a5-65319decd230)


*Timing Diagram*


(i)F1

![WhatsApp Image 2024-12-24 at 11 31 18_d5fe2e14](https://github.com/user-attachments/assets/ee4db4d7-ad7c-4c1d-a56f-a67ca595a774)

(ii)F2


![Screenshot 2024-12-27 135411](https://github.com/user-attachments/assets/5a19da84-edc6-4faa-aa1f-401be7a35dab)


*Result:*

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
