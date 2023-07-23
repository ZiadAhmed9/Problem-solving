[Problem link](https://www.hackerrank.com/challenges/sock-merchant/problem?isFullScreen=true&h_r=next-challenge&h_v=zen&h_r=next-challenge&h_v=zen)
### Solution
```C
void take(int* arr,int size)
{
    int i;
    for(i=0;i<size;i++)
    {
        scanf("%d",arr+i);
    }
}

int main(void)
{
    int i,count=0,size;
    int colors[100]={0};
    scanf("%d",&size);    
    int* pile=(int*)malloc(size*sizeof(int));  
    take(pile,size);    
    for(i=0;i<size;i++)
    {
        colors[pile[i]]++;
    }
    for(i=0;i<100;i++)
    {
            count=count+(colors[i]/2);
    }
    printf("%d",count);
}
```

