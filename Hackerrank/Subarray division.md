[Problem link](https://www.hackerrank.com/challenges/the-birthday-bar/problem?isFullScreen=true)
![[Pasted image 20230723174858.png]]
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
int birthday(int* arr,int size,int d,int m)
{
    int i,j,count=0,sum=0;
    for(i=0;i<=size-m;i++)
    {
        for(j=i;j<i+m;j++)
        {
            sum=sum+arr[j];
        }
        if(sum==d)
        {
            count++;
        }
        sum=0;
    }
    return count;
}

int main(void)
{
    int size,d,m;
    scanf("%d",&size);
    int* arr=(int*)malloc(size*sizeof(int));
    take(arr,size);
    scanf("%d%d",&d,&m);
    printf("%d",birthday(arr,size,d,m));
}
```

