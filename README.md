
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
    char ch1, ch2, ch3;

    
    printf("Enter first character: ");
    scanf(" %c", &ch1);
    printf("Enter second character: ");
    scanf(" %c", &ch2);
    printf("Enter third character: ");
    scanf(" %c", &ch3);

    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);

    return 0;
}
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/85f245c9-a645-4f87-b9fe-0b50236c56f2)
















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
    printf("Enter a value: ");
    scanf("%d", &A);

    if (A > 0) {
        printf("%d is a positive number.\n", A);
    } else if (A == 0) {
        printf("%d is zero.\n", A);
    } else {
        printf("%d is a negative number.\n", A);
    }

    return 0;
}

```

# OUTPUT:
![image](https://github.com/user-attachments/assets/dd238fe7-3b9c-4db6-8524-9c28ff0cc2b5)











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
    float num1, num2, min;

    printf("Enter first fraction number: ");
    scanf("%f", &num1);
    printf("Enter second fraction number: ");
    scanf("%f", &num2);

    min = (num1 < num2) ? num1 : num2;

    printf("Minimum number: %.2f\n", min);

    return 0;
}

```

## OUTPUT:
![image](https://github.com/user-attachments/assets/e0d3a5f3-e19f-457b-ab50-b00502e2bbc4)










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

    printf("Enter a value: ");
    scanf("%d", &num);

    if (num == 1) {
        printf("The input value is equal to 1.\n");
    }

    return 0;
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/3dd14024-259c-496a-b3aa-fe228cd95adf)










	

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
    float sub1, sub2, sub3, total, percentage;
    int min_marks = 40;

    printf("Enter marks of subject 1: ");
    scanf("%f", &sub1);
    printf("Enter marks of subject 2: ");
    scanf("%f", &sub2);
    printf("Enter marks of subject 3: ");
    scanf("%f", &sub3);

    total = sub1 + sub2 + sub3;
    percentage = (total / 300) * 100;

    if (sub1 >= min_marks && sub2 >= min_marks && sub3 >= min_marks) {
        if (percentage >= 60) {
            printf("Division: First\n");
        } else if (percentage >= 45 && percentage < 60) {
            printf("Division: Second\n");
        } else {
            printf("Division: Pass\n");
        }
    } else {
        printf("Division: Fail\n");
    }

    printf("Total marks: %.2f\n", total);
    printf("Percentage: %.2f%%\n", percentage);

    return 0;
}

```

## OUTPUT:

![image](https://github.com/user-attachments/assets/72580738-9a62-493f-8053-e11333cfb02c)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

