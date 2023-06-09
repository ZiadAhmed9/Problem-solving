[Problem link]()
### Solution
```C
#include <stdio.h>
#include <stdlib.h>
#define size_of_variable 32
int main()
{
    unsigned int x=0xf0;
    int bit=0,i=0;
    while(i<size_of_variable)
    {
        if((x>>i)&1)
        {
            bit=i;
            break;
        }
        i++;
    }
    printf("%d",bit);
    return 0;
}
```

