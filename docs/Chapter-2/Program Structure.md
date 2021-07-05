# Program Structure
In this chapter, we will study in depth, the Arduino program structure and we will learn more new terminologies used in the Arduino world. The Arduino software is open-source. The source code for the Java environment is released under the GPL and the C/C++ microcontroller libraries are under the LGPL.

**Sketch** − The first new terminology is the Arduino program called **“sketch”**.

## Structure
Arduino programs can be divided in three main parts: **Structure, Values** (variables and constants), and **Functions**. In this tutorial, we will learn about the Arduino software program, step by step, and how we can write the program without any syntax or compilation error.

Let us start with the Structure. Software structure consist of two main functions −

- Setup( ) function
- Loop( ) function

![Structure](img\structure.png)



```c++
void setup ( ) {

}
```

**PURPOSE** − The **setup()** function is called when a sketch starts. Use it to initialize the variables, pin modes, start using libraries, etc. The setup function will only run once, after each power up or reset of the Arduino board.

```c++
void loop ( ) {
  
}
```

**PURPOSE** − After creating a **setup()** function, which initializes and sets the initial values, the **loop()** function does precisely what its name suggests, and loops consecutively, allowing your program to change and respond. Use it to actively control the Arduino board.

# Data Types

Data types in C refers to an extensive system used for declaring variables or functions of different types. The type of a variable determines how much space it occupies in the storage and how the bit pattern stored is interpreted.

The following table provides all the data types that you will use during Arduino programming.

| void | Boolean       | char  | Unsigned char | byte   | int   | Unsigned int      | word          |
| ---- | ------------- | ----- | ------------- | ------ | ----- | ----------------- | ------------- |
| long | Unsigned long | short | float         | double | array | String-char array | String-object |

## void

The void keyword is used only in function declarations. It indicates that the function is expected to return no information to the function from which it was called.

### Example
```c++
Void Loop ( ) {
   // rest of the code
}
```
## Boolean

A Boolean holds one of two values, true or false. Each Boolean variable occupies one byte of memory.

### Example
```c++
boolean val = false ; // declaration of variable with type boolean and initialize it with false
boolean state = true ; // declaration of variable with type boolean and initialize it with true
}
```

## Char

A data type that takes up one byte of memory that stores a character value. Character literals are written in single quotes like this: 'A' and for multiple characters, strings use double quotes: "ABC".

However, characters are stored as numbers.This means that it is possible to do arithmetic operations on characters, in which the ASCII value of the character is used. For example, 'A' + 1 has the value 66, since the ASCII value of the capital letter A is 65.

### Example
```c++
Char chr_a = ‘a’ ;//declaration of variable with type char and initialize it with character a
Char chr_c = 97 ;//declaration of variable with type char and initialize it with character 97
```
## Unsigned char

Unsigned char is an unsigned data type that occupies one byte of memory. The unsigned char data type encodes numbers from 0 to 255.


### Example
```c++
Unsigned Char chr_y = 121 ; // declaration of variable with type Unsigned char and initialize it with character y
```
## byte

A byte stores an 8-bit unsigned number, from 0 to 255.


### Example
```c++
byte m = 25 ;//declaration of variable with type byte and initialize it with 25
```
## int

Integers are the primary data-type for number storage. int stores a 16-bit (2-byte) value. This yields a range of -32,768 to 32,767 (minimum value of -2^15 and a maximum value of (2^15) - 1).

The int size varies from board to board. On the Arduino Due, for example, an int stores a 32-bit (4-byte) value. This yields a range of -2,147,483,648 to 2,147,483,647 (minimum value of -2^31 and a maximum value of (2^31) - 1).


### Example
```c++
int counter = 32 ;// declaration of variable with type int and initialize it with 32
```
## Unsigned int

Unsigned ints (unsigned integers) are the same as int in the way that they store a 2 byte value. Instead of storing negative numbers, however, they only store positive values, yielding a useful range of 0 to 65,535 (2^16) - 1). The Due stores a 4 byte (32-bit) value, ranging from 0 to 4,294,967,295 (2^32 - 1).


### Example
```c++
Unsigned int counter = 60 ; // declaration of variable with type unsigned int and initialize it with 60
```

## Word

On the Uno and other ATMEGA based boards, a word stores a 16-bit unsigned number. On the Due and Zero, it stores a 32-bit unsigned number.


### Example
```c++
word w = 1000 ;//declaration of variable with type word and initialize it with 1000
```


## Long

Long variables are extended size variables for number storage, and store 32 bits (4 bytes), from -2,147,483,648 to 2,147,483,647.


### Example
```c++
Long velocity = 102346 ;//declaration of variable with type Long and initialize it with 102346
```

## unsigned long

Unsigned long variables are extended size variables for number storage and store 32 bits (4 bytes). Unlike standard longs, unsigned longs will not store negative numbers, making their range from 0 to 4,294,967,295 (2^32 - 1).


### Example
```c++
Unsigned Long velocity = 101006 ;// declaration of variable with type Unsigned Long and initialize it with 101006
```
## short

A short is a 16-bit data-type. On all Arduinos (ATMega and ARM based), a short stores a 16-bit (2-byte) value. This yields a range of -32,768 to 32,767 (minimum value of -2^15 and a maximum value of (2^15) - 1).


### Example
```c++
short val = 13 ;//declaration of variable with type short and initialize it with 13
```
## float

Data type for floating-point number is a number that has a decimal point. Floating-point numbers are often used to approximate the analog and continuous values because they have greater resolution than integers.

Floating-point numbers can be as large as 3.4028235E+38 and as low as -3.4028235E+38. They are stored as 32 bits (4 bytes) of information.


### Example
```c++
float num = 1.352;//declaration of variable with type float and initialize it with 1.352
```
## double

On the Uno and other ATMEGA based boards, Double precision floating-point number occupies four bytes. That is, the double implementation is exactly the same as the float, with no gain in precision. On the Arduino Due, doubles have 8-byte (64 bit) precision.


### Example
```c++
double num = 45.352 ;// declaration of variable with type double and initialize it with 45.352
```




