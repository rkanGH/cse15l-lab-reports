# Week 4 Lab Report
<br>
<br>
<br>
<br>

## Code Change #1
Original Code: [Link](https://github.com/ucsd-cse15l-w22/markdown-parse/blob/main/MarkdownParse.java)
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

