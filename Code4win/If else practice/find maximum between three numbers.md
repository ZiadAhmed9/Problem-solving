[Problem link](https://codeforwin.org/c-programming/c-program-to-find-maximum)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x,y,z,max=0;
    scanf("%d%d%d",&x,&y,&z);
    max=x;
    if(y>max)
    {
        max=y;
    }
    else if(z>max)
        max=z;
        printf("Maximum = %d",max);
    return 0;
}

```

