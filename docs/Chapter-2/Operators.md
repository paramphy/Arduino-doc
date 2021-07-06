An operator is a symbol that tells the compiler to perform specific mathematical or logical functions. C language is rich in built-in operators and provides the following types of operators −

- Arithmetic Operators
- Comparison Operators
- Boolean Operators
- Bitwise Operators
- Compound Operators

# Arithmetic Operators

| Operator name       | Operator simple | Description                                                  | Example             |
| ------------------- | --------------- | ------------------------------------------------------------ | ------------------- |
| assignment operator | =               | Stores the value to the right of the equal sign in the variable to the left of the equal sign. | A = B               |
| addition            | +               | Adds two operands                                            | A + B will give 30  |
| subtraction         | -               | Subtracts second operand from the first                      | A - B will give -10 |
| multiplication      | *               | Multiply both operands                                       | A * B will give 200 |
| division            | /               | Divide numerator by denominator                              | B / A will give 2   |
| modulo              | %               | Modulus Operator and remainder of after an integer division  | B % A will give 0   |

### Example

```c++
void loop () {
   int a = 9,b = 4,c;
   c = a + b;
   c = a - b;
   c = a * b;
   c = a / b;
   c = a % b;
}
```

### Result

```
a + b = 13
a - b = 5
a * b = 36
a / b = 2
Remainder when a divided by b = 1
```

# Comparison Operators

Assume variable A holds 10 and variable B holds 20 then 

| Operator name            | Operator simple | Description                                                  | Example              |
| ------------------------ | --------------- | ------------------------------------------------------------ | -------------------- |
| equal to                 | ==              | Checks if the value of two operands is equal or not, if yes then condition becomes true. | (A == B) is not true |
| not equal to             | !=              | Checks if the value of two operands is equal or not, if values are not equal then condition becomes true. | (A != B) is true     |
| less than                | <               | Checks if the value of left operand is less than the value of right operand, if yes then condition becomes true. | (A < B) is true      |
| greater than             | >               | Checks if the value of left operand is greater than the value of right operand, if yes then condition becomes true. | (A > B) is not true  |
| less than or equal to    | <=              | Checks if the value of left operand is less than or equal to the value of right operand, if yes then condition becomes true. | (A <= B) is true     |
| greater than or equal to | >=              | Checks if the value of left operand is greater than or equal to the value of right operand, if yes then condition becomes true. | (A >= B) is not true |

### Example

```c++
void loop () { 
   int a = 9,b = 4
   bool c = false;
   if(a == b)
      c = true;
   else
      c = false;

   if(a != b)
      c = true;
   else
      c = false;
   
   if(a < b)
      c = true;
   else
      c = false;
   
   if(a > b)
      c = true;
   else
      c = false;
   
   if(a <= b)
      c = true;
   else
      c = false;
   
   if(a >= b)
      c = true;
   else
      c = false;
}
```

### Result

```
c = false
c = true
c = false
c = true
c = false
c = false
```

# Boolean Operators

Assume variable A holds 10 and variable B holds 20 then −

| Operator name | Operator simple | Description                                                  | Example            |
| ------------- | --------------- | ------------------------------------------------------------ | ------------------ |
| and           | &&              | Called Logical AND operator. If both the operands are non-zero then then condition becomes true. | (A && B) is true   |
| or            | \|\|            | Called Logical OR Operator. If any of the two operands is non-zero then then condition becomes true. | (A \|\| B) is true |
| not           | !               | Called Logical NOT Operator. Use to  reverses the logical state of its operand. If a condition is true then  Logical NOT operator will make false. | !(A && B) is false |

### Example

```c++
void loop () {
   int a = 9,b = 4
   bool c = false;
   if((a > b)&& (b < a))
      c = true;
   else
      c = false;

   if((a == b)|| (b < a))
      c = true;
   else
      c = false;

   if( !(a == b)&& (b < a))
      c = true;
   else
      c = false;
}
```

### Result

```
c = true
c = true
c = true
```

# Bitwise Operators

Assume variable A holds 60 and variable B holds 13 then −

| Operator name | Operator simple | Description                                                  | Example                                  |
| ------------- | --------------- | ------------------------------------------------------------ | ---------------------------------------- |
| and           | &               | Binary AND Operator copies a bit to the result if it exists in both operands. | (A & B) will give 12 which is 0000 1100  |
| or            | \|              | Binary OR Operator copies a bit if it exists in either operand | (A \| B) will give 61 which is 0011 1101 |
| xor           | ^               | Binary XOR Operator copies the bit if it is set in one operand but not both. | (A ^ B) will give 49 which is 0011 0001  |
| not           | ~               | Binary Ones Complement Operator is unary and has the effect of 'flipping' bits. | (~A ) will give -60 which is 1100 0011   |
| shift left    | <<              | Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand. | A << 2 will give 240 which is 1111 0000  |
| shift right   | >>              | Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand. | A >> 2 will give 15 which is 0000 1111   |

### Example

```c++
void loop () {
   int a = 10,b = 20
   int c = 0;
   c = a & b ;
   c = a | b ;
   c = a ^ b ;
   c = a ~ b ;
   c = a << b ;
   c = a >> b ; 
}
```

### Result

```
c = 12
c = 61
c = 49
c = -60
c = 240
c = 15
```

# Compound Operators

Assume variable A holds 10 and variable B holds 20 then −

| Operator name           | Operator simple | Description                                                  | Example                           |
| ----------------------- | --------------- | ------------------------------------------------------------ | --------------------------------- |
| increment               | ++              | Increment operator, increases integer value by one           | A++ will give 11                  |
| decrement               | --              | Decrement operator, decreases integer value by one           | A-- will give 9                   |
| compound addition       | +=              | Add AND assignment operator. It adds right operand to the left operand and assign the result to left operand | B += A is equivalent to B = B+ A  |
| compound subtraction    | -=              | Subtract AND assignment operator. It subtracts right operand from the left operand and assign the result to left operand | B -= A is equivalent to B = B - A |
| compound multiplication | *=              | Multiply AND assignment operator. It multiplies right operand with the left operand and assign the result to left operand | B*= A is equivalent to B = B* A   |
| compound division       | /=              | Divide AND assignment operator. It divides left operand with the right operand and assign the result to left operand | B /= A is equivalent to B = B / A |
| compound modulo         | %=              | Modulus AND assignment operator. It takes modulus using two operands and assign the result to left operand | B %= A is equivalent to B = B % A |
| compound bitwise or     | \|=             | bitwise inclusive OR and assignment operator                 | A \|= 2 is same as A = A \| 2     |
| compound bitwise and    | &=              | Bitwise AND assignment operator                              | A &= 2 is same as A = A & 2       |

### Example

```c++
void loop () {
   int a = 10,b = 20
   int c = 0;
   
   a++;
   a--;
   b += a;
   b -= a;
   b *= a;
   b /= a;
   a %= b;
   a |= b;
   a &= b;
}
```

### Result

```
a = 11
a = 9
b = 30
b = 10
b = 200
b = 2
a = 0
a = 0
a = 30
```

## 
