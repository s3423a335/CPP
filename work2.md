# cpp_work2-1:(2018/04/17)
```
#include <iostream>
#include <iomanip>
using namespace std;
int fun(int array[3][3])
{
	int i,j,t;
	for(i=0;i<3;i++)
		for(j=0;j<i;j++)
		{
			t=array[i][j];
			array[i][j]=array[j][i];
			array[j][i]=t;
		}
		return 0;
}
int main()
{
	int i,j;
	int array[3][3]={{1,2,3},{4,5,6},{7,8,9}};
	cout << "轉換前" <<endl;
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;j++)
			cout << setw(7) << array[i][j] ;
		cout<< endl;
	}
	fun(array);
	cout << "轉換後" <<endl;
	for(i=0;i<3;i++)
	{
		for(j=0;j<3;j++)
			cout << setw(7) << array[i][j] ;
		cout<< endl;
	}
    return 0;
}

```
![image](https://github.com/s3423a335/cpp/blob/master/02.PNG)

# cpp_work2-2:(2018/04/17)
```
#include<iostream>
using namespace std;
int main()
{
	int i;
	char array[12];
	array[0]='a';
	array[1]='b';
	array[2]='b';
   //	array[12]='c';
	printf("%s\n",array);
    return 0;
}
```
![image](https://github.com/s3423a335/cpp/blob/master/03.PNG)
