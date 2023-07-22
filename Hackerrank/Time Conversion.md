[Problem link](https://www.hackerrank.com/challenges/one-week-preparation-kit-time-conversion/problem?h_l=interview&isFullScreen=true&playlist_slugs%5B%5D%5B%5D=preparation-kits&playlist_slugs%5B%5D%5B%5D=one-week-preparation-kit&playlist_slugs%5B%5D%5B%5D=one-week-day-one)
### Solution
```C
char* timeConversion(char* s) {
    char* str=malloc(8*sizeof(char));
    for(int i=0;i<8;i++)
    {
        str[i]=s[i];
    }
    if(s[8]=='A'&&s[0]=='1'&&s[1]=='2')
    {
        str[0]-=1;
        str[1]-=2;
    }
    else if(s[8]=='P'&&s[0]!='1'&&s[1]!='2') {
    str[0]+=1;
    str[1]+=2;
    }
    return str;
}
```

