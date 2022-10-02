---
title: site1
date: 2022-07-28 20:26:06
tags: sort
categories: c++
type: about
---

## 插入排序

```c++
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
```

