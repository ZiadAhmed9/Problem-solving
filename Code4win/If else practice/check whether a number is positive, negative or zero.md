[Problem link](https://codeforwin.org/c-programming/c-program-to-check-negative-positive-zero)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x;
    scanf("%d",&x);
    if(x>0)
    {
        printf("number is positive");
    }
    else if (x==0)
    {
        printf("number is 0");
    }
    else
    {
        printf("number is negative");
    }
    return 0;
}

```

