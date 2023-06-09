[Problem link](https://codeforwin.org/c-programming/c-program-to-print-number-of-days-in-month#program-to-print-days-in-a-month-using-array)
### Solution

```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    const int number_of_days[12]={31,28,31,30,31,30,31,31,30,31,30,31};
    int x;
    scanf("%d",&x);
    printf("Number of days in month number %d is %d",x,number_of_days[x-1]);

    return 0;
}

```

