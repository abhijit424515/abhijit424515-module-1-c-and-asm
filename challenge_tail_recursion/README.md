# Assembly, but limited memory!

One of these other days we came across a 64-bit device on which anything consuming too much memory would just blow up! For some reason, @Owl-A wanted this device to compute Fibonacci numbers and due to the limited memory, he had to program directly in Assembly. Good people write good codes and thus, [Owl-A's%20script](fib.S) is not working. 

Someone informed him that memory was the source of all his troubles but he, being occupied with other things, has now left it to you to figure out how to make things work! He mentioned something of the likes of [Tail Recursion](https://en.wikipedia.org/wiki/Tail_call) before leaving but we are not sure how this would help...

## Instructions

Running `python3 emulator.py` without any arguments ends up reading the `fib.S`; `python3 emulator.py -` reads the assembly from your standard input (NOTE that the assembly input must be followed by `$` on a new line) ; and `python3 emulator.py file.S` reads the assembly from `file.S`. None of the `.py` files or the `template.S` file are required to be read/understood. You only need to understand `fib.S` and reimplement it in such a manner that the memory consumed is now lower!

Setting the [enivornment variable](https://en.wikipedia.org/wiki/Environment_variable) `DEBUG` with the value `"yes"` would allow you to debug your script by providing you additional information.

The **real** flag can be obtained by connecting to the server using `nc cybersecclub.cse.iitb.ac.in 5000` with IITBVPN; and then submitting your assembly input followed by a `$` on a new line. It will take a while to execute, possibly a minute or two, so be patient!

You needn't try to understand any of the `.py` files or the `template.S` file. Upload your final solution script in [solve.py](solve.py) along with the correct flag.
