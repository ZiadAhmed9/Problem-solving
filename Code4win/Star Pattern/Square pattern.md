[Problem link](https://codeforwin.org/c-programming/square-star-pattern-in-c)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>


void square_pattern(char n)
{
    char i,j;
    for(i=0;i<n;i++)
    {
        for(j=0;j<n;j++)
            printf("*");
        printf("\n");
    }

}

int main()

    square_pattern(5);


    return 0;
}



```

