# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE:03/09/2025
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1. Start the program.
2. Declare a character variable and a pointer to it.
3. Read a character from the user through the pointer.
4. Check if the character is a vowel (a, e, i, o, u or A, E, I, O, U). 
5. Display whether it is a vowel or a consonant.  

## Program:
#include <stdio.h>

int main() {
    char ch, *p;
    p = &ch;

    printf("Enter a character: ");
    scanf("%c", p);

    if (*p == 'a' || *p == 'e' || *p == 'i' || *p == 'o' || *p == 'u' ||
        *p == 'A' || *p == 'E' || *p == 'I' || *p == 'O' || *p == 'U') {
        printf("'%c' is a vowel\n", *p);
    } else {
        printf("'%c' is a consonant\n", *p);
    }

    return 0;
}


## Output:

<img width="1534" height="685" alt="image" src="https://github.com/user-attachments/assets/afbdccb6-0f52-4018-a09e-d8374491f1e3" />


## Result:
Thus the program was executed and the output was verified successfully.
