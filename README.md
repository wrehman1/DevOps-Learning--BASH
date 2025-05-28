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

![image](https://github.com/user-attachments/assets/a047be16-af51-452b-883d-c212263662ce) 

![image](https://github.com/user-attachments/assets/54e9efc3-a156-437f-be7a-d098fb63130a)


**If Statements**

If statements allow you to make decisions and execute different code blocks based on conditions. Conditions are formed using comparison operators and logical operators. You can compare numbers, strings and combine conditions using logical operators and else clauses. 

![image](https://github.com/user-attachments/assets/752eb978-fb81-4afa-a58f-0f5cf225302f)

![image](https://github.com/user-attachments/assets/b3d5ea07-fddb-49ef-a9f8-44973a9b0e29)


**Else and Elif Statements**

The else clause provides an alternative code block to be executed when the if condition is false. When this condition is false, we look at the elif condition, otherwise we resort to the else clause which executes the command. Therefore the else clause is used in conjunction with the if statement and can be combined with the LFQ word for more complex conditions. This adds flexibility and versatility to the bash group, which allows us to handle alternative paths based on the condition evaluation. 

![image](https://github.com/user-attachments/assets/0eb349db-2154-4a6e-b601-488483a5ba67)

![image](https://github.com/user-attachments/assets/2e0ea27a-6669-478a-84a9-fa0f7c4c25f8)


**Nested if Statements**

Nested if statements offer the following benefits: 
- They allow the evaluation of multiple conditions and execution of clde blocks based on the results.
- They provide a way to handle complex decision making scenarios.
- They enhance the flexibility & versatility of bash groups, which means its easy to adapt to different situations.

- ![image](https://github.com/user-attachments/assets/05627d2c-0b09-4546-a2bc-1d5aca543a5b)


**While Loops**

While loops allow you to repeatedly execute a block of code as long as a condition is true. The condition is evaluated before each iteration. THe loop continues until the condition becomes false. While loops are useful for automating tasks and iterating over data.

![image](https://github.com/user-attachments/assets/0308b788-48de-4d49-b0b6-ef552a1c4b59)

![image](https://github.com/user-attachments/assets/fa9545e1-c5d2-4c28-bdf2-a3a43233dd4c)


**For loops**

For loops are used to iterate over a sequence or a range of values. The variable in the loop takes on each value in the sequence and the code block in between the do and done keywords is executed for each iteration. For loops can be used with arrays, lists of values or ranges to automate repetitive tasks and process data systematically. 

![image](https://github.com/user-attachments/assets/d226387f-e56a-4cc3-a80b-28892ac1add0)

![image](https://github.com/user-attachments/assets/641a4bf2-53d2-43e1-937f-b9afe0209f04)

![image](https://github.com/user-attachments/assets/785dcfe9-691b-48f9-be91-cd660528f9b3)


**Break and continue**

The break statement exits the innermost loop it is placed in. The continue statement skips the rest of the current iteration for the loop and moves onto the next iteration. Both break and continue statements can be used with "for" and "while" loops to fine tune the behaviour of the loops

![image](https://github.com/user-attachments/assets/c226ac6f-cb78-4faf-9104-d2c8f9a569ad)

![image](https://github.com/user-attachments/assets/6192b0ef-86c6-494b-8254-ca7c672c8ef0)

![image](https://github.com/user-attachments/assets/2ee4afe3-d4ca-457c-b28f-a6eaf9fd1ffc)


**Basics of Functions**

Functions are defined using the function bame followed by parentheses and then curly braces. They are then encapsulate the code within the curly braces. Functions can be called using the function name and we can exit parameters to make them more flexible and reuseable.

![image](https://github.com/user-attachments/assets/a0596c11-56d2-440c-a935-b257beebfc68)

![image](https://github.com/user-attachments/assets/82cfa195-bfe7-4d06-a1bc-30c7c360b69b)


**Parameters**

Positional parameters allow us to pass data to functions and access them using numbered variables like "$1 and $2". Special parameters provide additional information about the script and the arguements passed to it, such as "$#" for number of arguments, "$0" for name of script amd "$@" for all arguments. These are known as special parameters. 

![image](https://github.com/user-attachments/assets/02f81c8d-273a-4cd7-ac8e-9ba63533651f)


**User Inputs**

The read command is useful for interactive prompts, allowing users to enter information within the script. Commands and arguments provide a direct way to pass user input when calling functions. By combining both methods, we can create functions that offer flexibilty in how the user input is accepted. We explored different methods of accepting user input within functions in bash scripting and by leveraging user input, we are able to create interactive and versatile scripts that cater to specific user needs. 

![image](https://github.com/user-attachments/assets/2d95f58e-ed6e-48be-b080-4902a3a24bf5)

![image](https://github.com/user-attachments/assets/00d92017-cde4-4343-8279-d5500a4a057e)


**Handling Bad Data**

Conditional statements can be used to validate user inputs ensuring they meet the desired criteria. Exit codes can be leveraged to determine the success or failure of input validation and provide appropriate feedback to the user. WE can use input sanitization such as parameter expansion with patent substitution, which can help clean and transform user inputs to meet the required format of constraints. 

![image](https://github.com/user-attachments/assets/2061d75d-628c-42ec-a28a-d21b03f74ed5)

![image](https://github.com/user-attachments/assets/69acaaf7-e36b-40a7-98bf-62dc230ffa08)


**Piping**

Piping allows us to pass the output of one command as in input for another comman using the pipe symbol. Piping within functions enables us to perform advanced data operations and store the results in variables. We can combine piping with other commands or functions to create more complex data manipulations pipleines.

![image](https://github.com/user-attachments/assets/f9b519ef-9a58-4a1f-91cf-67301d3ba470)


**Set -e**

Using Set -e can help catch errors as soon as they happen and avoid unexpected behaviour due to unhandled errors. Not all non-zero exit codes are indicative of error that should stop the script. 

![image](https://github.com/user-attachments/assets/aa3b5ebf-b473-4e8b-8cd3-e53689b21ef3)


**Set -u**

Using Set -u prevents the script from running into potential problems due to missing data.

![image](https://github.com/user-attachments/assets/325e160d-0fe4-44ff-ad22-6b3c9df7e7f8)


**Reading Environment Variables**

Understanding how to read environment variables is essential, but it's also important to be familiar with some commonly used standard environment variables that provide useful information. 

![image](https://github.com/user-attachments/assets/276113c7-7c1b-4e7a-99ba-134f118860f8)




![image](https://github.com/user-attachments/assets/ac6e3835-c8bd-483d-99cb-1b5844d6d74d)


