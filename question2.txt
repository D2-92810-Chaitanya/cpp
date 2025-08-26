// Factorial of a number

#include <stdio.h>

int fact(int n)
{
    if (n == 0 || n == 1)
        return 1;

    else
        return n * fact(n - 1);
}

int main()
{

    int n;
    printf("enter a number: ");
    scanf("%d", &n);

    if (n < 0)
    {
        printf("factorial does not exist for negative");
    }
    else
    {

        int result = fact(n);

        printf("%d! = %d", n, result);
    }
}
