[Problem link](https://www.hackerrank.com/challenges/one-week-preparation-kit-mini-max-sum/problem?h_l=interview&isFullScreen=true&playlist_slugs%5B%5D%5B%5D=preparation-kits&playlist_slugs%5B%5D%5B%5D=one-week-preparation-kit&playlist_slugs%5B%5D%5B%5D=one-week-day-one&h_r=next-challenge&h_v=zen)
### Solution
```C
void miniMaxSum(int arr_count, int* arr) {
    unsigned long int min=4294967295,max=0,temp_min=0,temp_max=0;
    for(int i=0;i<arr_count;i++)
    {
        for(int j=0;j<arr_count;j++)
        {
            if(j==i)
            {
                continue;
            }
            temp_max+=arr[j];
            temp_min+=arr[j];
        }
        if(temp_max>max)
        max=temp_max;
        if(temp_min<min)
        min=temp_min;
        temp_min=0;
        temp_max=0;
    }
    printf("%ld %ld",min,max);
}
```

