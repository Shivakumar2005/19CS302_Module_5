# EX 21 C program to calculate the area of a triangle using pointer.
## DATE:03/09/2025
## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
1. Start the program.
2. Declare three float variables to store base, height, and area of the triangle.
3. Assign pointers to base, height, and area variables.
4. Read the base and height from the user through pointers. 
5. Calculate the area using the formula (*area) = 0.5 * (*base) * (*height) and display the result.  

## Program:
#include <stdio.h>

int main() {
    float base, height, area;
    float *b, *h, *a;

    b = &base;
    h = &height;
    a = &area;

    printf("Enter base of the triangle: ");
    scanf("%f", b);

    printf("Enter height of the triangle: ");
    scanf("%f", h);

    *a = 0.5 * (*b) * (*h);

    printf("Area of the triangle = %.2f\n", *a);

    return 0;
}


## Output:

<img width="1580" height="665" alt="image" src="https://github.com/user-attachments/assets/9db6105e-028c-4c4a-8c6e-4b74ed7faca6" />


## Result:
Thus the program was executed and the output was verified successfully.
