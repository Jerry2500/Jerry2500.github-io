---
title: site2
date: 2022-07-29 20:40:11
categories: c++
type: site
---

## 二进制转化

```c++
void printbin(int num)
{
	stack<int>st;
	while(!st.empty())
	st.pop();
	while(num>0)
	{
		st.push(num%2);
		num/=2;
	}
	while(!st.empty())
	{
		cout<<st.top();
		st.pop();
	}
	
}
```

