# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
#include <stdio.h>
#include <math.h>

// Function to calculate EMI (without return type)
void calculateEMI(float principal, float rate, int months) {
    // Convert the rate into a monthly interest rate
    rate = rate / 12 / 100;
    
    // Calculate the EMI using the formula
    float emi = (principal * rate * pow(1 + rate, months)) / (pow(1 + rate, months) - 1);
    
    // Display the EMI
    printf("The EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;
    
    // Read principal amount, rate of interest, and months
    printf("Enter principal amount: ");
    scanf("%f", &principal);
    
    printf("Enter rate of interest (annual): ");
    scanf("%f", &rate);
    
    printf("Enter number of months: ");
    scanf("%d", &months);
    
    // Call the function to calculate EMI
    calculateEMI(principal, rate, months);
    
    return 0;
}

## OUTPUT
![Screenshot 2025-04-28 195405](https://github.com/user-attachments/assets/8ffc03d7-504f-4595-8f8f-b829bae7beb0)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
#include <stdio.h>

int main() {
    int n = 6;
    int first = 0, second = 1, next;

    printf("Fibonacci Series up to %d terms:\n", n);
    
    // Print first two terms
    printf("%d, %d, ", first, second);
    
    for (int i = 3; i <= n; i++) {
        next = first + second;
        printf("%d, ", next);
        
        // Update terms
        first = second;
        second = next;
    }
    
    return 0;
}
## OUTPUT
![Screenshot 2025-04-28 195519](https://github.com/user-attachments/assets/2fae083a-5c32-4d2a-b2cd-70cb5983349c)








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM!
#include <stdio.h>

int main() {
    int n;
    
    // Read the number of elements
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    int arr[n];
    
    // Input elements into the array
    printf("Enter the elements:\n");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Print the last element of the array
    printf("The last element is: %d\n", arr[n-1]);
    
    return 0;
}

## OUTPUT

![Screenshot 2025-04-28 195626](https://github.com/user-attachments/assets/0f94a997-1e20-4c21-836c-10f5a4efb83d)








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
#include <stdio.h>

int main() {
    int n, count = 0;
    
    // Read the number of elements
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    int arr[n];
    
    // Input array elements
    printf("Enter the elements:\n");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Count positive elements
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    
    // Display the result
    printf("Total positive elements: %d\n", count);
    
    return 0;
}

## OUTPUT
![Screenshot 2025-04-28 195844](https://github.com/user-attachments/assets/c5c5ddbb-d836-4349-877c-768397871ee1)





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
#include <stdio.h>

int main() {
    int n;
    
    // Read size of the array
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    
    int arr[n];
    
    // Input elements of the array
    printf("Enter the elements:\n");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Replace even elements with 'E'
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replace even elements with 'E'
        }
    }
    
    // Display updated array
    printf("Updated array:\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    
    return 0;
}
## Output:
 
![Screenshot 2025-04-28 195959](https://github.com/user-attachments/assets/3acc1a98-fb74-46f7-89ef-5fe3f9c55deb)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



