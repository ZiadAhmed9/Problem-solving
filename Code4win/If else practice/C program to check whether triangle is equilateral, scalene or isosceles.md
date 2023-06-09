[Problem link](https://codeforwin.org/c-programming/c-program-to-check-whether-triangle-is-equilateral-isosceles-scalene)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int side1, side2, side3;
    scanf("%d%d%d",&side1,&side2,&side3);
    if((side2==side3)&&(side1==side2))
    {
        printf("The triangle is equilateral Triangle");
    }
    else if((side1==side2)||(side2==side3)||(side3==side1))
    {
        printf("The triangle is isosceles ");
    }
    else
        printf("Th triangle is scalene");
    return 0;
}

```

