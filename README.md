# C-Session
Dedicated folder for learning C
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main()
{
    int n, g;

    srand(time(0));
    n = rand() % 100 + 1;

    printf("Guess the random number (1-100):\n");

    do
    {
        scanf("%d", &g);

        if(g > n)
        {
            printf("Too high! Try again.\n");
        }
        else if(g < n)
        {
            printf("Too low! Try again.\n");
        }
        else
        {
            printf("Congrats! You guessed it.\n");
        }

    } while(g != n);

    return 0;
}
