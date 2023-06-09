[Problem link](https://codeforwin.org/c-programming/c-program-to-set-nth-bit-of-number-using-bitwise-operator)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    unsigned char x=0b00010101;
    int n;
    scanf("%d",&n);
    x|=(1<<n);
    printf("%d",x);
    return 0;
}

```

