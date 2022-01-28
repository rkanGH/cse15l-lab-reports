# Week 4 Lab Report
<br>
<br>
<br>
<br>

Original Code: [Link](https://github.com/ucsd-cse15l-w22/markdown-parse/blob/main/MarkdownParse.java)

## Code Change #1

![Image](c3.png)
The error inducing input: [test2.md](https://raw.githubusercontent.com/rkanGH/cse15l-lab-reports/main/lab%202/test2.md)
<br>
When the code is run with the input this is the error that is induced:
![Image](c4.png)
<br>
<br>
This error is occuring when we have text at the end of the last link. This is because when `currentIndex` is set to `closeParen` it is set as the index of the last `)`. However, there is a character after the last `)` which means `currentIndex` will always be less than `markdown.length` and the while loop will run forever. 
<br>

To summarize, the failure-inducing input of having a character after the last `)` resulted in bug in the code of not checking if there were any characters after the last `)` which led to the symptom of the while loop running forever.

<br>
<br>
<br>
<br>

## Code Change #2

![Image](new.png)
The error inducing input: [test.md](https://raw.githubusercontent.com/rkanGH/cse15l-lab-reports/main/lab%202/test.md)

<br>
Although the code compiles and runs when the file is run, it produces the image's link which isn't what we want.
<br>
The original code has the output:
<br>
<br>

![Image](c6.png)
<br>
However, we do not want the `.png` link we want the code to only output the html link:
<br>
<br>

![Image](c7.png)

This error occurs because the code prints anything that is in the parenthesis with the markdown format. 

<br>
<br>
To summarize, the error inducing input of an image link resulted in the bug of not checking whether or not a link is actually in the parenthesis which then led to the code printing out the link that wasn't an actual link.
<br>
<br>
<br>
<br>

## Code Change #3

![Image](new1.png)

The error inducing input: 
