# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
## DATE:03/09/2025
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1. Start the program.
2. Define a structure with members: empno, dept, and basic pay.
3. Declare an array of 3 structures to store employee details.
4. Read empno, dept, and basic pay of each employee. 
5. Calculate Gross Salary = Basic Pay + (10% of BP) + (30% of BP) and display details.  

## Program:
#include <stdio.h>

struct Employee {
    int empno;
    char dept[20];
    float bp, gross;
};

int main() {
    struct Employee emp[3];
    int i;

    for (i = 0; i < 3; i++) {
        printf("\nEnter details of employee %d\n", i + 1);
        printf("Employee Number: ");
        scanf("%d", &emp[i].empno);
        printf("Department: ");
        scanf("%s", emp[i].dept);
        printf("Basic Pay: ");
        scanf("%f", &emp[i].bp);

        emp[i].gross = emp[i].bp + (0.1 * emp[i].bp) + (0.3 * emp[i].bp);
    }

    printf("\nEmployee Details with Gross Salary:\n");
    for (i = 0; i < 3; i++) {
        printf("\nEmployee %d\n", i + 1);
        printf("Emp No: %d\n", emp[i].empno);
        printf("Department: %s\n", emp[i].dept);
        printf("Basic Pay: %.2f\n", emp[i].bp);
        printf("Gross Salary: %.2f\n", emp[i].gross);
    }

    return 0;
}


## Output:

<img width="1847" height="693" alt="image" src="https://github.com/user-attachments/assets/79c8ba6a-25a2-4297-9c36-3a031df76e15" />


## Result:
Thus the program was executed and the output was verified successfully.
