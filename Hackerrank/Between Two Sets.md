[Problem link](https://www.hackerrank.com/challenges/between-two-sets/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)
![[Pasted image 20230722195443.png]]
### Solution
```C
int getTotalX(int a_count, int* a, int b_count, int* b) {

    int j,i,num,count=0,flag=0,flag1=0;

    for(num=1;num<=100;num++)

    {

        for(i=0;i<a_count;i++)

        {

            if(num%a[i]==0)

            {

                flag++;

            }

        }

    if(flag==a_count)

    {

        for(j=0;j<b_count;j++)

        {

            if(b[j]%num==0)

            {

                flag1++;

            }

        }

    }

    if(flag1==b_count)

    {

        count++;

    }

    flag=0;

    flag1=0;

    }

    return count;

}
```

