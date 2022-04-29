#include <stdio.h>

int main()
{
    //Prime numbers = A prime number (or a prime) is a natural number greater than 1 and is not a product of two samller natural numbers.
    // Disclaimer : This is not the best method to solve this problem
    int n, i, prime = 0;
    printf("Enter the number which is to be checked \n");
    scanf("%d", &n);
    for (i = 2; i < n; i++)
    {
        if (n % i == 0)
        {
            prime = 1;
            break;
        }
    }
    if (prime == 1)
    {
        printf("The number is a non-prime\n");
    }
    else
    {
        printf("The number is a prime \n");
    }
    return 0;
}
