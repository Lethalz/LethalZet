# Understading Pipes and redirection 

You can use the `>` to redirect standard output to be saved to a file instead of being sent to STDOUT

***If we redirect to a file which does not exist, it will be created automatically for us. If we save into a file which already exists, however, then it's contents will be cleared, then the new output saved to it.***

If you want the file that you're redirecting to, to keep its data you can append the new data by using the `>>` operator

## Redirecting from a file (STDIN)

If i use the `<` operator i can send infomation the other way meaning send info from a file to a program for example:

```sh
User@bash:cat myoutput
2+2
User@bash:bc < myoutput
4
```
## Standard error

STDERR is one of the three possible streams
* Standard in (STDIN)
* Standard out(STDOUT)
* Standard ERR(STDERR)

The three streams have numbers associated with them STDERR is stream number 2  comparted to STDOUT which is 1

**if we place a number before the `>` operator it will redirect that stream**

`User@bash:ls -l video.mpg blah.foo 2> errors.txt`

If we wished to save both the standard error and standard output messages into a file;

We could do that by redirecting the STDERR to the STDOUT and > to a File.

`User@bash:ls -l video.mpg blah.fooo > file1.txt 2>&1`

## Piping

The `|` Operator feeds the output from the program on the left as input to the program on the right.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; You can pipe as many programs as you'd like. The UNIX approch to computing prides itself on having everything work seemlessly together


`USER@bash: ls | head -3 | tail -1`


You can combine pipes and redirection too dont be afraid to try and mix these two.






 
