完成一个判断整数是否素数的函数，即，输入一个整数，判断其是否素数
```markdown
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
