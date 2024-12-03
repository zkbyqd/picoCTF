# binhexa [100]
---
![image](https://github.com/HAW-THL/Write-ups/assets/80387757/10245860-207e-49d6-8ec2-f2c0ab6968ed)

- With the command from the task you land on a Netcat server that lets you calculate binary operations

```shell
nc titan.picoctf.net 62274  

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 11000001
Binary Number 2: 00111111


Question 1/6:
Operation 1: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
```

- In the first task, you have to perform a left shift by adding a 0 to the right end of the number, so the result is 110000010

```shell
Enter the binary result: 110000010
Correct!

Question 2/6:
Operation 2: '&'
Perform the operation on Binary Number 1&2.
```
- In the second task, you have to perform an AND operation that checks bit by bit whether both corresponding digits are 1. The result is therefore 00000001

```shell
Enter the binary result: 00000001
Correct!

Question 3/6:
Operation 3: '*'
Perform the operation on Binary Number 1&2.
```
- In the 3rd task, a multiplication is to be carried out. We used an online calculator for this, the result is 10111101111111

```shell
Enter the binary result: 10111101111111
Correct!

Question 4/6:
Operation 4: '+'
Perform the operation on Binary Number 1&2.
```
- In the 4th task you have to carry out an addition. We also used an online calculator for this. The result is 100000000

```shell
Enter the binary result: 100000000
Correct!

Question 5/6:
Operation 5: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
```
- In the 5th task, you have to perform a right shift, which works like the left shift, only to the right, so that the rightmost digit is omitted. The result is therefore 00011111

```shell
Enter the binary result: 00011111
Correct!

Question 6/6:
Operation 6: '|'
Perform the operation on Binary Number 1&2.

```
- In the 6th task, you should use the bitwise OR operation, which always results in 1 if at least one of the digits in the respective bit is 1. The result is therefore 11111111

```shell
Enter the binary result: 11111111
Correct!

Enter the results of the last operation in hexadecimal: ff
```
- At the end, we have to enter the result of task 6 in hexadecimal. To do this, you can divide the number into blocks of four and convert each into a hexadecimal digit. 1111 is the highest possible hexadecimal digit, i.e. f. The result is therefore ff and we get the flag on input

```shell
Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_6ab1ad84}
```
