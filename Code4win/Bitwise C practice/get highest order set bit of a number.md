[Problem link](https://codeforwin.org/c-programming/c-program-to-get-highest-order-set-bit-of-number)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>
#define size_of_variable 32
int main()
{
    unsigned int x=-1;
    int bit=0,i=0;
    while(i<size_of_variable)
    {
        if((x>>i)&1)
            bit=i;
        i++;
    }
    printf("%d",bit);
    return 0;
}
```

