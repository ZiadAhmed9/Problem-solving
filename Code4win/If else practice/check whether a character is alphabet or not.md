[Problem link](https://codeforwin.org/c-programming/c-program-to-check-alphabet)
### Solution
Note: take the input as character
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    char x;
    scanf("%c",&x);
    if((x>='a')&&(x<='z'))
    {
        printf("you entered letter %c",(char)x);
    }
    else if(x>='A'&&x<='Z')
    {
        printf("you entered letter %c",(char)x);
    }
    else
        printf("input is not a letter");
    return 0;
}

```

