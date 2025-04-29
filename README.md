
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
	#include <stdio.h>

	int main() {
   	 char ch1, ch2, ch3;

	    // Read characters one by one
	    printf("Enter first character: ");
	    scanf(" %c", &ch1);
	
	    printf("Enter second character: ");
	    scanf(" %c", &ch2);
	
	    printf("Enter third character: ");
	    scanf(" %c", &ch3);
	
	    // Print in reverse order
	    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
	
	    return 0;
	}

## OUTPUT:

![Screenshot 2025-04-29 154159](https://github.com/user-attachments/assets/9ec3c229-d3da-466f-af35-9f6043fb645e)


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

	#include <stdio.h>
	
	int main() {
	    int A;
	
	    // Read the value of A
	    printf("Enter a number: ");
	    scanf("%d", &A);
	
	    // Check if A is positive
	    if (A > 0) {
	        printf("A is a positive number.\n");
	    } else {
	        printf("A is not a positive number.\n");
	    }
	
	    return 0;
}

# OUTPUT:

![Screenshot 2025-04-29 154636](https://github.com/user-attachments/assets/4ccee651-a4bc-4f90-a3ed-cfbdc9f0ec9c)

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

	#include <stdio.h>
	int main(){
	    int a,b,min;
	    scanf("%d%d",&a,&b);
	    min=(a<b)?a:b;
	    printf("Minimum between %d and %d is %d",a,b,min);
	}

## OUTPUT:

![image](https://github.com/user-attachments/assets/5d618bff-f8e2-4faa-b2c8-eefae0ffa4e0)

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

#include <stdio.h>

int main() {
    int value;

    // Read input value
    printf("Enter a number: ");
    scanf("%d", &value);

    // Check if value is equal to 1
    if (value == 1) {
        printf("The value is equal to 1.\n");
    }

    return 0;
}


## OUTPUT:

![Screenshot 2025-04-29 155441](https://github.com/user-attachments/assets/f5d10753-1a69-43ec-97c9-15bc939a6562)



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

#include <stdio.h>
int main()  
{
    int m1,m2,m3,total;
    float percentage;
    scanf("%d%d%d",&m1,&m2,&m3);
    total = m1 + m2 + m3;
    percentage = (float)total / 3;
    printf("Total Marks = %d\n",total);
    printf("Percentage = %.2f\n",percentage);
    
    if (m1 >= 40 && m2 >= 40 && m3 >= 40)
    {
        if (percentage >= 60)
        {
            printf("Division = First");
        }
        else if(percentage < 60 && percentage >= 48)
        {
            printf("Division = Second");
        }
        else if(percentage < 48 && percentage >= 36)
        {
            printf("Division = Pass");
        }
        else
        {
            printf("Division = Fail");
        }
    }else
    {
        printf("Division = Fail");
    }
    return 0;
}

## OUTPUT:

![Screenshot 2025-04-29 155649](https://github.com/user-attachments/assets/8d1f805d-14b6-4d0a-82c8-e9f0587c511d)

## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

