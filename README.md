
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    char a, b, c;

    printf("Enter first character: ");
    scanf(" %c", &a);

    printf("Enter second character: ");
    scanf(" %c", &b);

    printf("Enter third character: ");
    scanf(" %c", &c);

    printf("\nCharacters in reverse order: %c %c %c\n", c, b, a);

    return 0;
}
```

## OUTPUT:













<img width="663" height="150" alt="Screenshot 2025-10-31 170102" src="https://github.com/user-attachments/assets/5427f1d2-6de3-4c87-8653-ac1375c3b515" />




## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include <stdio.h>

int main() {
    int A;

    printf("Enter a number: ");
    scanf("%d", &A);

    if (A > 0) {
        printf("%d is a positive number.\n", A);
    } else if (A < 0) {
        printf("%d is not a positive number.\n", A);
    } else {
        printf("The number is zero.\n");
    }

    return 0;
}
```

# OUTPUT:

<img width="696" height="73" alt="Screenshot 2025-10-31 170226" src="https://github.com/user-attachments/assets/f8fc3721-8133-4f00-9232-3ff56bbaf615" />










# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>

int main() {
    float a, b, min;

    printf("Enter first number: ");
    scanf("%f", &a);

    printf("Enter second number: ");
    scanf("%f", &b);

    // Using ternary operator to find the minimum
    min = (a < b) ? a : b;

    printf("The minimum number is: %.2f\n", min);

    return 0;
}
```

## OUTPUT:



<img width="677" height="98" alt="Screenshot 2025-10-31 170323" src="https://github.com/user-attachments/assets/1572e8f2-cb4e-4b08-ac9b-f173c37a0f20" />






## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>

int main() {
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num == 1) {
        printf("The number is equal to 1.\n");
    }

    return 0;
}
```

## OUTPUT:


<img width="562" height="74" alt="Screenshot 2025-10-31 170436" src="https://github.com/user-attachments/assets/bc303255-e979-4171-9c91-95c818832e60" />







	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
```
#include <stdio.h>

int main() {
    float m1, m2, m3, total, percentage;

    printf("Enter marks of three subjects:\n");
    scanf("%f %f %f", &m1, &m2, &m3);

    total = m1 + m2 + m3;
    percentage = total / 3;

    printf("\nTotal Marks = %.2f\n", total);
    printf("Percentage = %.2f%%\n", percentage);

    // Check if student has failed any subject (below 35)
    if (m1 < 35 || m2 < 35 || m3 < 35) {
        printf("Result: Fail (one or more subjects below 35)\n");
    } 
    else {
        if (percentage >= 60)
            printf("Result: First Division\n");
        else if (percentage >= 45)
            printf("Result: Second Division\n");
        else if (percentage >= 35)
            printf("Result: Pass Division\n");
        else
            printf("Result: Fail\n");
    }

    return 0;
}
```

## OUTPUT:
<img width="679" height="177" alt="Screenshot 2025-10-31 170543" src="https://github.com/user-attachments/assets/787fcc52-b7b8-4415-ba35-e74e5535e58d" />


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.
