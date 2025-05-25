# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
~~~
 #include <stdio.h>
 #include <stdlib.h>
 #include <time.h>
 int main() {
    int n, i, lower, upper;
    srand(time(0));
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &n);
    printf("Enter the lower limit: ");
    scanf("%d", &lower);
    printf("Enter the upper limit: ");
    scanf("%d", &upper);
    printf("Generated random numbers:\n");
    for (i = 0; i < n; i++) {
        int random_num = (rand() % (upper - lower + 1)) + lower;
        printf("%d\n", random_num);
    }
    return 0;
 }

~~~

# OUTPUT:
![image](https://github.com/user-attachments/assets/c0c5d512-0f8c-4184-9985-bfbefd4ed0eb)


# RESULT:
 Thus the program is created and executed successfully

