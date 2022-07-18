完成一个函数，输入值为整数，输出该值的二进制
```markdown
#include<iostream>
#include<stack>
using namespace std;
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
int main()
{
	int num;
	cin>>num;
	printbin(num);
	return 0;
}
  ```
