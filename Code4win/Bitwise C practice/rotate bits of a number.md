[Problem link](https://codeforwin.org/c-programming/c-program-rotate-number-bits)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>
#define size_of_variable 8
int main()
{
    char x=-15,temp;
    int count=0,i=0,n;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        if(x&0b10000000)
            temp=1;
        else
            temp=0;
        x=x<<1;
        x|=temp;
    }
    printf("%d",x);
    return 0;
}
```

