
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
    char c1, c2, c3;

    scanf(" %c %c %c", &c1, &c2, &c3);

    printf("Characters in reverse order: %c %c %c\n", c3, c2, c1);

    return 0;
}

```

## OUTPUT:
<img width="1917" height="875" alt="Screenshot 2025-10-19 164302" src="https://github.com/user-attachments/assets/376f8a54-dff8-48a5-9548-c17ceb23752d" />

















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
    scanf("%d",&A);

   if(A>0){
       printf("%d is a Positive Number");
   }else{
       printf("%d is a Negavite Number");
   }
    return 0;
}

```

# OUTPUT:

<img width="1918" height="872" alt="Screenshot 2025-10-19 164701" src="https://github.com/user-attachments/assets/32345093-5ede-4cfd-9d23-c5902c5f0886" />










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
    float n1, d1, n2, d2, f1, f2, rt;

    printf("Enter the numerator of the first fraction: ");
    scanf("%f", &n1);
    printf("Enter the denominator of the first fraction: ");
    scanf("%f", &d1);
    printf("Enter the numerator of the second fraction: ");
    scanf("%f", &n2);
    printf("Enter the denominator of the second fraction: ");
    scanf("%f", &d2);

    f1 = n1 / d1;
    f2 = n2 / d2;

    rt = (f1 < f2) ? f1 : f2;

    printf("The smaller (minimum) fraction value is: %.2f\n", rt);

    return 0;
}

```

## OUTPUT:

<img width="1918" height="882" alt="Screenshot 2025-10-19 165234" src="https://github.com/user-attachments/assets/bae17bee-3235-4d6b-9604-c7b401eab096" />








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
int main(){
    int n;
    scanf("%d",&n);
    
    if(n==1){
        printf("The  Number is equal to one");
    }else{
        printf("The Number is Not equal to one");
    }
}
```

## OUTPUT:
<img width="1918" height="868" alt="Screenshot 2025-10-19 165637" src="https://github.com/user-attachments/assets/f73d7cfd-e298-45b8-8d08-5d0e233dd29c" />









	

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
int main(){
    int m1,m2,m3;
    scanf("%d %d %d",&m1,&m2,&m3);
    int tol = m1+m2+m3;
    float per= tol/3;
    
    printf("Total is %d\n",tol);
    printf("Percentage is %.2f",per);
    
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60)
            printf("\nDivision = First");
        else if (per >= 48)
            printf("\nDivision = Second");
        else if (per >= 36)
            printf("\nDivision = Pass");
    } 
    else {
        printf("\nDivision = Fail");
    }
}

```

## OUTPUT:
<img width="1918" height="866" alt="Screenshot 2025-10-19 170454" src="https://github.com/user-attachments/assets/e8a16328-510d-4941-ad5d-784e77706af4" />

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

