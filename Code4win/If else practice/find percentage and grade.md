[Problem link](https://codeforwin.org/c-programming/c-program-to-enter-student-marks-and-calculate-percentage-and-grade)
### Solution
```C
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int phy,chem,bio,math,comp;
    float total;
    scanf("%d%d%d%d%d",&phy,&chem,&bio,&math,&comp);
    if(((phy<=100)&&(phy>=0))&&((chem<=100)&&(chem>=0))&&((bio<=100)&&(bio>=0))&&((math<=100)&&(math>=0))&&((comp<=100)&&(comp>=0)))
    {
        total=(phy+chem+bio+math+comp)/5;
        if(total>=90&&total<=100)
            printf("Percentage is %f \n grade A",total);
        else if(total>=80&&total<90)
            printf("Percentage is %f \n grade B",total);
        else if(total>=70&&total<80)
            printf("Percentage is %f \n grade C",total);
        else if(total>=80&&total<60)
            printf("Percentage is %f \n grade D",total);
        else if(total>=60&&total<=40)
            printf("Percentage is %f \n grade E",total);
        else
            printf("percentage is %f \n grade F",total);
    }
    else
        printf("error");
    return 0;
}

```

