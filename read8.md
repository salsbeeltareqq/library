[Home](https://sayefdeen.github.io/reading-notes/home)

# Operators and Loops.

In any condition, there is usually one **operator** and two **operands**, The operands are placed on each side of the operator, they can be values of variables, You often see expressions enclosed in brackets.

`(score >= Pass)`

- `()` Enclosing brackets
- `score` Operand
- `pass` Operand
- `>=` Conditional Operator

`((5 < 2 ) && (2 >= 3))`

- `(5 < 2)` Expression 1
- `(2 >= 3)` Expression 2
- `&&` Logical Operator

| Condition 1 | Logical Operator | Condition 2 | Result |
| ----------- | ---------------- | ----------- | ------ |
| True        | `&&`             | True        | True   |
| True        | `&&`             | False       | False  |
| False       | `&&`             | False       | False  |
| True        | `||`             | True        | True   |
| True        | `||`             | False       | True   |
| False       | `||`             | False       | False  |

## 2. Loops

Loops check a condition, if it returns true, a code block will run, Then the condition will be checked again and if it still returns true, the code block will run again. It repeatsuntil the condition returns false, There are three commone types of loops.

A . For Loop : if you need to run a code a specifi number of times.

B . While Loop : if you need to run a code but you don't know how many time

C . Do While : this will run the code inside the loop at least **one time** before checking the condition.

`for ( var i = 0; i< 10 ; i++){document.write()}`

`for` : keyword
`(var i =0;i<10;i++)`: condition (counter)
`document.write()`: code to execure during loop
`var i = 0` initializing the counter

`i < 10` condition if it get to false the loop will stop.

`i++` incremant to increase the counter.

Example of while loop:

```javascript
var i = 1;
var msg = "";
while (i < 10) {
  msg += i + " x 5 =" + i * 5 + "<br>";
  i++;
}
document.write("<p>" + msg + "</p>");
```

this code will print Multipication Table for 5

1 x 5 = 5<br>
2 x 5 = 10<br>
3 x 5 = 15<br>
4 x 5 = 20<br>
5 x 5 = 25<br>
6 x 5 = 30<br>
7 x 5 = 35<br>
8 x 5 = 40<br>
9 x 5 = 45<br>

and it will wtop @ 10



## 1. Comparison operators evauating conditions.

| Symbol | Name                  | Job                                                                     |
| ------ | --------------------- | ----------------------------------------------------------------------- |
| ==     | Is Equal To           | compares two values to see if they are the same                         |
| !=     | Is Not Equal To       | compares two values to see if they are not the same                     |
| ===    | Strict Equal To       | compares two values and cheack there data type if they are the same     |
| !==    | Strict Not Equal To   | compares two values and cheack there data type if they are not the same |
| >      | Grater than           | checks if the number on the left is greater than on the right           |
| <      | Less than             | checks if the number on the left is less than on the right              |
| >=     | greater than or equal | checks if the number on the left is greater than or equal on the right  |
| <=     | less than or equal    | checks if the number on the left is less than or equal on the right     |