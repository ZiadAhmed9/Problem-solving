[Problem link](https://www.hackerrank.com/challenges/apple-and-orange/problem?isFullScreen=true)
### Solution
![[Pasted image 20230619221031.png]]
```C
void countApplesAndOranges(int s, int t, int a, int b, int apples_count, int* apples, int oranges_count, int* oranges) {

    int apples_res=0,oranges_res=0,position;
    for(int i=0;i<apples_count;i++)
    {
        position=a+apples[i];
        if(position<=t&&position>=s)
        {
            apples_res++;
        }
    }
    for(int i=0;i<oranges_count;i++)
    {
        position=b+oranges[i];
        if(position<=t&&position>=s)
        {
            oranges_res++;
        }
    }
    printf("%d\n%d",apples_res,oranges_res);
}
```

