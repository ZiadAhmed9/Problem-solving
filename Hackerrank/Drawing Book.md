[Problem link](https://www.hackerrank.com/challenges/drawing-book/problem?isFullScreen=true)
### Solution
```C
int pageCount(int n, int p) 
{
    int i,count=0;
    if(p<=1)
    {
        return count;
    }
    else if(p>n/2)
    {
        for(i=n;i>n/2;i=i-2)
        {
            if(i==p||(i-1)==p)
            {
                if(p==(n-1)&&(n%2==0))
                count++;
                return count;
            }
            else 
            {
                count++;
            }
        }
    }
    else if(p<=n/2)
    {
        count++;
        for(i=2;i<=n/2;i=i+2)
        {
            if(i==p||(i+1)==p)
            {
                return count;
            }
            else {
                count++;
            }
        }
    }
    return 0;
}
```

