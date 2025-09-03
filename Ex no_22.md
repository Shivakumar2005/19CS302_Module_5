# EX 22 C program to count total number of even elements in an array using calloc().
## DATE:03/09/2025
## AIM:
To write a C program to count total number of even elements in an array using calloc().

## Algorithm
1. Start the program.
2. Declare a pointer to hold the array and a variable for size.
3. Allocate memory dynamically for the array using calloc().
4. Read array elements from the user and check each element for evenness. 
5. Count the even numbers and display the total.  

## Program:
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *arr, n, i, count = 0;

    printf("Enter number of elements: ");
    scanf("%d", &n);

    arr = (int *)calloc(n, sizeof(int));

    printf("Enter %d elements: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", arr + i);
    }

    for (i = 0; i < n; i++) {
        if (*(arr + i) % 2 == 0) {
            count++;
        }
    }

    printf("Total even elements = %d\n", count);

    free(arr);
    return 0;
}


## Output:

<img width="1815" height="677" alt="image" src="https://github.com/user-attachments/assets/d5b1f142-258e-47eb-a158-00ddd218c279" />


## Result:
Thus the program was executed and the output was verified successfully.
