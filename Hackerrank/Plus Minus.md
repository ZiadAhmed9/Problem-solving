[Problem link](https://www.hackerrank.com/challenges/one-week-preparation-kit-plus-minus/problem?h_l=interview&isFullScreen=true&playlist_slugs%5B%5D%5B%5D=preparation-kits&playlist_slugs%5B%5D%5B%5D=one-week-preparation-kit&playlist_slugs%5B%5D%5B%5D=one-week-day-one)
### Solution
```C
void plusMinus(int arr_count, int* arr) {
    int pos=0,neg=0,zeros=0;
    float perPos,perNeg,perZero;
    for(int i=0;i<arr_count;i++)
    {
        if (arr[i]>0)
        {
            pos++;
        }
        else if(arr[i]<0)
        neg++;
        else
        zeros++;
    }
    perPos=(float)pos/arr_count;
    perNeg=(float)neg/arr_count;
    perZero=(float)zeros/arr_count;
    printf("%0.6f\n%0.6f\n%0.6f",perPos,perNeg,perZero);
}
```

