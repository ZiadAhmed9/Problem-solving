[Problem link](https://www.hackerrank.com/challenges/kangaroo/problem?isFullScreen=true)
### Solution
```C
char* kangaroo( int x1, int v1, int x2, int v2)

{
    static char s[]="YES";
    static char s2[]="NO";
    if(v2>v1)
    {
        return s2;
    }
    else if(x1==x2)
    {
        return s;
    }
    else
    {
        while(x1<=x2)
    {
        if(x2==x1)
            return s;
        x1=x1+v1;
        x2=x2+v2;
    }
    }
    return s2;
}
```
![[Pasted image 20230722175649.png]]
