# DevOps-Learning--BASH

**Shebang Line**

Shebang is also known has the #bang which is a crucial tool in the execution of the bash script. 
**#!/bin/bash** is known as the "shebang line" and serves as the directive to the operating system on how to interpret the script.
In this case, we are asking the operating system to interpret the script using the binary bash. 
The "!" denotes to the specific interpretor on whcih shell should handle the script. 
To show this, I created a new file "touch greet.sh. Then I edited the file by going in "vi greet.sh". I added the text starting with the shebang line. ":wq!" saved and exited the file. Then ensured the script was executable by adding "chmod +x greet.sh". Then when the command "./ greet.sh" was ran, it would give the output of the message in the file. 

![image](https://github.com/user-attachments/assets/bfcfb06b-db6d-423a-939a-1b3cc8fca399)


**Comments**

Comments are lines in the script that are not executed as part of the code. Instead they serve as informative text for us to read the script. 
Adding comments to the script is considered as best practice because it helps you and others to understand the purpose, functionality and logic of the script.
To add comments, it always begins with "#".
Comments are added in the vim editor in this case, it is with the extension.sh file. 
Comments are made within the "'" quotation marks.

![image](https://github.com/user-attachments/assets/9c8e71d0-b5e3-493d-ad64-a441986bbe62)

![image](https://github.com/user-attachments/assets/f9919a81-58ac-45f7-83de-77fb3ce485de)


**Run scripts from anywhere**

To a run a script from anywhere on the terminal; it should be placed in commom directory which is user local bin, this can be seem using the "scho $PATH" command. 
To move a script to another directory, it needs a super user comman "sudo". It also needs to have execution rights which can be altared via "sudo chmod +x /usr/local/bin/greet" command.  

![image](https://github.com/user-attachments/assets/63f2c441-dae8-4ba2-b3cb-51bb12d0a0be)


**Variables**

Variables are an essential component of bash scripting as they allow you to store and manipulate data. It makes the script dynamic and flexible. Variables are created using the assignemnt operator equals (=). To access the value of a variable, we propend the name of the variable with a dollar sign ($). Variables can hold different types of data such as strings, numbers and arrays. Variable interpolation allows you to use variables within strings to create a dynamic output

![image](https://github.com/user-attachments/assets/0fac58b0-53e7-4945-8250-df1e29e56eb7)

![image](https://github.com/user-attachments/assets/490ff411-2f7e-4135-aeeb-47e5b9909b55)

![image](https://github.com/user-attachments/assets/ca005b38-fd8f-49a6-b646-6b13ea45827f)


**Parameters**

Parameters are provided after a script name when executing a script. Inside the script, parameters can be accessed using "$1, $2, $3" based on their position. The special variable dollar can be used to access all the parameters passed to the script. By allowing inputs through parameters you can make your script more interactive and versatile.

![image](https://github.com/user-attachments/assets/95a2b37a-7cc5-46d4-a979-fca95f7a056a)

![image](https://github.com/user-attachments/assets/190f3f33-f938-4e2c-bd71-d57a124d2442)

![image](https://github.com/user-attachments/assets/d31b2940-ca39-49d8-ae11-f72bb167487f)

![image](https://github.com/user-attachments/assets/5e8cf3a7-c211-4080-8bee-17e732b181f6)


**Arithmetic Expansion**

Arithmetic expansion provides the following benefits: 

* It enables mathematical calculations and expression evaluation within the bash script.
* It allows the incorporation of variables and parameters into the calculation, making the script more dynamic and flexible.
* It provides a concise and readable syntax using the dollar and double parentheses notation.

![image](https://github.com/user-attachments/assets/24798e7c-753e-4b28-b496-4795a909fcb8) ![image](https://github.com/user-attachments/assets/f74413af-2c5a-42d8-a96e-4a74bfd86099)

![image](https://github.com/user-attachments/assets/6470bb0f-bc0f-4593-b228-aa905143debc) ![image](https://github.com/user-attachments/assets/950ea0de-5ef6-42c3-8181-0ee580861e6b)


**Arithemetic Expansion (with Parameters)**

This enables us to create dynamic scripts that can accept user input and perform calculations based on those inputs

![image](https://github.com/user-attachments/assets/a047be16-af51-452b-883d-c212263662ce) ![image](https://github.com/user-attachments/assets/54e9efc3-a156-437f-be7a-d098fb63130a)


**If Statements**


![image](https://github.com/user-attachments/assets/752eb978-fb81-4afa-a58f-0f5cf225302f)



