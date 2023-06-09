[Problem link](https://codeforwin.org/c-programming/c-program-to-check-leap-year)
Leap year: a leap year is divisible by 100 and 4
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x;
    scanf("%d",&x);
    if((x%100!=0)&&(x%4==0))
        printf("The year is a leap year");
    else
        printf("It is not a leap year");
    return 0;
}

```

