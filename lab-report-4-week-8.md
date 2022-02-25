# Week 8 Lab Report
<br>

## Repository Links:
[My Repository](https://github.com/rkanGH/markdown-parse)
<br>
[Repository I reviewed](https://github.com/leo3friedman/markdown-parse)
<br>
<br>

## Snippet #1:
<br>
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)

<br>

### Snippet #1 Test:

![Image](47.png)

<br>
My implementation failed:

![Image](44.png)

<br>

The Implementation I reviewed failed:

![Image](41.png)

<br>
<br>

## Snippet #2:
<br>
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)

### Snippet #2 Test:

![Image](48.png)

<br>
My implementation failed:

![Image](45.png)

<br>

The Implementation I reviewed failed:

![Image](42.png)

<br>
<br>

## Snippet #3:
<br>
[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
    https://ucsd-cse15l-w22.github.io/
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text

### Snippet #3 Test:

![Image](49.png)

<br>
My implementation failed:

![Image](46.png)

<br>

The Implementation I reviewed failed:

![Image](43.png)
<br>
<br>

## Questions:
1. 