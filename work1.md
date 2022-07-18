写一个插入排序的函数，即输入一个数组，完成排序

```markdown
#include<iostream>
using namespace std;
void insertion_sort(int arr[], int len)
{
    int i,j,key;
    for (i=1;i<len;i++)
	{
        key = arr[i];
        j=i-1;
        while((j>=0) && (arr[j]>key)) 
		{
            arr[j+1] = arr[j];
            j--;
        }
        arr[j+1] = key;
    }
}
int main()
{
	int arr[2000]={0};
	int len=0;
	cin>>len;//输入数组长度
	for(int i=0;i<len;i++)
	cin>>arr[i];
    insertion_sort(arr, len);
    for(int i = 0; i < len; i++)
    cout<<arr[i]<<" ";
    return 0;
}
```
