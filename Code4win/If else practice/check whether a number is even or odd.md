[Problem link](https://codeforwin.org/c-programming/c-program-to-check-even-odd)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int x;
    scanf("%d",&x);
    if(!(x%2))
        printf("The number is even");
    else
        printf("The number is odd");
    return 0;
}
```

