[Problem link](https://www.hackerrank.com/challenges/bon-appetit/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)
### Solution
```C
#include <stdio.h>
void take(int* arr,int size)
{
    int i;
    for(i=0;i<size;i++)
    {
        scanf("%d",arr+i);
    }
}
int main(void)
{
    int size,excluded_index,anna_charge,actual_price,i;
    scanf("%d%d",&size,&excluded_index);    //take size of bill and execluded
    int* bill=(int*)malloc(size*sizeof(int));   
    take(bill,size);    // take the bill
    scanf("%d",&anna_charge);   // take annas charge
    actual_price=0;
    for(i=0;i<size;i++)
    {
        if(i!=excluded_index)
        {
            actual_price=actual_price+bill[i];
        }
    
    if(actual_price/2==anna_charge)
    {
        printf("Bon Appetit");
    }
    else
        printf("%d",anna_charge-(actual_price/2));
}
```

