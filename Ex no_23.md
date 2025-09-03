# EX 23 C program to store and display the name, id, age and salary of an employee using structure(using array of structure).
## DATE:03/09/2025
## AIM:
To write a C program to store and display the name, id, age and salary of an employee using structure(using array of structure).

## Algorithm
1. Start the program.
2. Define a structure with members: name, id, age, and salary.
3. Declare an array of structures to store employee details.
4. Read details of employees from the user. 
5. Display the stored details of all employees.  

## Program:
#include <stdio.h>

struct Employee {
    char name[50];
    int id;
    int age;
    float salary;
};

int main() {
    int n, i;
    printf("Enter number of employees: ");
    scanf("%d", &n);

    struct Employee emp[n];

    for (i = 0; i < n; i++) {
        printf("\nEnter details of employee %d\n", i + 1);
        printf("Name: ");
        scanf("%s", emp[i].name);
        printf("ID: ");
        scanf("%d", &emp[i].id);
        printf("Age: ");
        scanf("%d", &emp[i].age);
        printf("Salary: ");
        scanf("%f", &emp[i].salary);
    }

    printf("\nEmployee Details:\n");
    for (i = 0; i < n; i++) {
        printf("\nEmployee %d\n", i + 1);
        printf("Name: %s\n", emp[i].name);
        printf("ID: %d\n", emp[i].id);
        printf("Age: %d\n", emp[i].age);
        printf("Salary: %.2f\n", emp[i].salary);
    }

    return 0;
}


## Output:

<img width="1820" height="677" alt="image" src="https://github.com/user-attachments/assets/7c4afd98-0fcf-4d51-a9c9-51c910d36e83" />


## Result:
Thus the program was executed and the output was verified successfully.
