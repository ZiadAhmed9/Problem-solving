[Problem link](https://codeforwin.org/c-programming/c-program-to-print-table-of-any-number)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>
#define size_of_variable 8
int main()
{
    unsigned char x;
    scanf("%d",&x);
    for(int i=0; i<=10; i++)
    {
        printf("%d * %d = %d\n",x,i,x*i);
    }
    return 0;
}



```

