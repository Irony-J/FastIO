# Fast IO For Competitive Programming

```cpp
#include <iostream>

void fastScan(int &num)
{
	bool negative = false;
	register int c;

	num = 0;

	c = getchar_unlocked();//getchar()

	if(c == '-'){
		negative = true;
		c = getchar();
	}

	for(; (c>='0' && c<='9');c=getchar_unlocked())
		num = num * 10 + c - '0';

	if(negative) num = - num;
	
}

int main(){

	int num;
	fastScan(num);
	printf("number is %d\n",num);
}
```





