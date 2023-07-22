[Problem link](https://www.hackerrank.com/challenges/migratory-birds/problem?h_r=profile)
### Solution
```C
int migratoryBirds(int arr_count,int* arr)
{
	int i,max=0,max_ind=0;
	int count[5]={0};
	for( i=0;i<arr_count;i++)
	{
		count[arr[i]]++;
		if(count[arr[i]]>max)
		{
		max=count[arr[i]];
		max_ind=i;
		}
		else if(count[arr[i]]==max&&arr[i]<arr[max_ind])
		max_ind=i;
	}
	return max;
}
```

