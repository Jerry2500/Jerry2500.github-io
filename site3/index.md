---
title: site3
date: 2022-07-29 20:51:32
categories: c++
type: tags
---

## 判断素数

```c++
#include<iostream>
#include<cmath>
using namespace std;
void judge(int num)
{
	bool is=1;
	for(int i=2;i<=sqrt(num);i++)
	{
		if(num%i==0)
		is=0;
	}
	if(is)cout<<num<<"是素数"<<endl;
	else cout<<num<<"不是素数"<<endl;
}
int main()
{
	int num;
	cin>>num;
	judge(num);
	return 0;
}
```

