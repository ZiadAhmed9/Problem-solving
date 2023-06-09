[Problem link](https://codeforwin.org/c-programming/c-program-to-find-maximum-between-two-numbers)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x,y;
    scanf("%d%d",&x,&y);
    if(x>y)
    {
        printf("Maximum = %d",x);
    }
    else if(x==y)
        printf("Both numbers are equal");
    else
        printf("Maximum = %d",y);
    return 0;
}

```

