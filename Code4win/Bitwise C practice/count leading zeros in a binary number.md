[Problem link](https://codeforwin.org/c-programming/c-program-to-count-leading-zeros-in-binary-number)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>
#define size_of_variable 32
int main()
{
    unsigned int x=2;
    int count=0,i=0;
    for(i=0;i<size_of_variable;i++)
    {
        if(!((x>>i)&1))
        {
            count++;
        }
        else count=0;
    }
    printf("%d",count);
    return 0;
}
```

