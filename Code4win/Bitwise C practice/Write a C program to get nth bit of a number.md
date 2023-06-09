[Problem link](https://codeforwin.org/c-programming/c-program-to-get-value-of-nth-bit-of-number)
note to get the bit we have more than on way but the second one is better
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num,n;
    scanf("%d%d",&num,&n);
    if((1<<n)&num)
        printf("The nth bit is %d",1);
    else
    printf("The nth bit is %d",0);
    return 0;
}



```

another solution

```c
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int num,n;
    for(;;)
    {
    scanf("%d%d",&num,&n);
    int bitstats=(num>>n)&1;
    printf("bit status is %d\n",bitstats);
    }
    return 0;
}
```


