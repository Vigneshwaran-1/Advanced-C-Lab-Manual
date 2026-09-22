EXP NO:2 C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION
Aim:
To write a C program for passing structure as function and returning a structure from a function

Algorithm:
1.	Define structure numbers with members a and b.
2.	Declare variable n of type numbers.
3.	Prompt the user to enter values for a and b.
4.	Input values for a and b into n using scanf.
5.	Call the add function with n as an argument.
6.	Print the result returned by the add function.
7.	Return 0
 
Program:
```
#include <stdio.h>

struct numbers {
    int a;
    int b;
};

// Function to add two numbers
struct numbers add(struct numbers n) {
    struct numbers result;
    result.a = n.a + n.b;   // store sum in 'a'
    result.b = 0;           // optional, unused
    return result;          // return structure
}

int main() {
    struct numbers n, ans;

    // Input values
    printf("Enter two numbers: ");
    scanf("%d %d", &n.a, &n.b);

    // Call function
    ans = add(n);

    // Output result
    printf("Sum = %d\n", ans.a);

    return 0;
}

```


Output:

```
Enter two numbers: 10 20
Sum = 30
```


Result:
Thus, the program is verified successfully
