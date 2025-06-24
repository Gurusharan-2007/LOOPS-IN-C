# LOOPS-IN-C
Some basic loop concept problems of C 

Loops Question
1. Print the first 10 natural numbers (1 to 10).

#include <stdio.h>

int main() {
    for (int i = 1; i <= 10; i++) {
        printf("%d\n", i);
    }
    return 0;
}

2. Print numbers from 0 to 10 and then from 10 to 0 (using two loops).

#include <stdio.h>

int main() {
    // First loop: 0 to 10
    for (int i = 0; i <= 10; i++) {
        printf("%d ", i);
    }
    printf("\n");
    for (int i = 10; i >= 0; i--) {
        printf("%d ", i);
    }
    return 0;
}

3. Print all even numbers from 1 to 20.

#include <stdio.h>

int main() {
    for (int i = 2; i <= 20; i += 2) {
        printf("%d ", i);
    }
    return 0;
}

4. Print the multiplication table for a given number (e.g., 5 × 1 to 5 × 10).

#include <stdio.h>

int main() {
    int num = 5;
    printf("Multiplication Table for %d:\n", num);
    for (int i = 1; i <= 10; i++) {
        printf("%d × %d = %d\n", num, i, num * i);
    }
    return 0;
}

5. Calculate the sum of the first 10 natural numbers.

#include <stdio.h>

int main() {
    int sum = 0;
    for (int i = 1; i <= 10; i++) {
        sum += i;
    }
    printf("The sum of the first 10 natural numbers is %d\n", sum);
    return 0;
}

6. Calculate the sum of numbers from 1 to n, where n is entered by the user.

#include <stdio.h>

int main() {
    int n, sum = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for (int i = 1; i <= n; i++) {
        sum += i;
    }
    printf("The sum of numbers from 1 to %d is %d\n", n, sum);
    return 0;
}

7. Read 10 numbers from the user and print their sum and average.

#include <stdio.h>

int main() {
    int numbers[10];
    int sum = 0;
    float average;
    printf("Enter 10 integers:\n");
    for (int i = 0; i < 10; i++) {
        printf("Number %d: ", i + 1);
        scanf("%d", &numbers[i]);
        sum += numbers[i];
    }
    average = sum / 10.0;
    printf("Sum = %d\n", sum);
    printf("Average = %.2f\n", average);
    return 0;
}

  8. Display the cube of numbers up to a given integer n (e.g., for n = 5, print cubes of 1 to 5).

#include <stdio.h>

int main() {
    int n;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    printf("Cubes of numbers from 1 to %d:\n", n);
    for (int i = 1; i <= n; i++) {
        printf("%d^3 = %d\n", i, i * i * i);
    }
    return 0;
}

9. Calculate the product of numbers from 1 to 5 (i.e., factorial 5!).

#include <stdio.h>

int main() {
    int product = 1;
    for (int i = 1; i <= 5; i++) {
        product *= i;
    }
    printf("The factorial of 5 is %d\n", product);
    return 0;
}

10. Calculate the factorial of a number entered by the user.

#include <stdio.h>

int main() {
    int n;
    unsigned long long factorial = 1;
    printf("Enter a non-negative integer: ");
    scanf("%d", &n);
    if (n < 0) {
        printf("Factorial is not defined for negative numbers.\n");
    } else {
        for (int i = 1; i <= n; i++) {
            factorial *= i;
        }
        printf("Factorial of %d is %llu\n", n, factorial);
    }
    return 0;
}

11. Keep asking the user to enter numbers until they enter 0, then print the sum of all positive numbers entered.

  #include <stdio.h>

int main() {
    int num, sum = 0;
    printf("Enter numbers (0 to stop):\n");
    do {
        printf("Enter a number: ");
        scanf("%d", &num);
        if (num > 0) {
            sum += num;
        }
    } while (num != 0);
    printf("The sum of all positive numbers entered is %d\n", sum);
    return 0;
}

12. Keep asking the user to enter a username until it is at least 8 characters long.

#include <stdio.h>
#include <string.h>

int main() {
    char username[100];
    do {
        printf("Enter a username (at least 8 characters): ");
        scanf("%s", username);
        if (strlen(username) < 8) {
            printf("Username too short. Please try again.\n");
        }
    } while (strlen(username) < 8);
      printf("Username accepted: %s\n", username);
   return 0;
}

13. Print a right-angled triangle of asterisks:

#include <stdio.h>

int main() {
    int i, j;
    for (i = 1; i <= 4; i++) {
        for (j = 1; j <= i; j++) {
            printf("*");
        }
        printf("\n");
    }
    return 0;
}


14. Print a right-angled triangle with numbers:
    

#include <stdio.h>

int main() {
    int i, j;
    for (i = 1; i <= 4; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d", j);
        }
        printf("\n");
    }
    return 0;
}

15. Print a right-angled triangle with repeated numbers:
    
#include <stdio.h>

int main() {
    int i, j;
    for (i = 1; i <= 4; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d", i);
        }
        printf("\n");
    }
    return 0;
}

16. Print the first 10 numbers of the Fibonacci sequence.

#include <stdio.h>

int main() {
    int n = 10;
    int a = 0, b = 1, next;
    printf("First %d numbers of the Fibonacci sequence:\n", n);
    for (int i = 1; i <= n; i++) {
        printf("%d ", a);
        next = a + b;
        a = b;
        b = next;
    }
    printf("\n");
    return 0;
}

    
