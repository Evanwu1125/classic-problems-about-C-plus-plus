输入一个整数 n，请你编写一个函数，int fact(int n)，计算并输出 n 的阶乘。

### 输入格式
共一行，包含一个整数 n。

### 输出格式
共一行，包含一个整数表示 n 的阶乘的值。

### 数据范围
1≤n≤10
### 输入样例：
3
### 输出样例：
6

```c++
#include <iostream>
#include <string>
using namespace std;

int fact(int n)
{   
    int count = 1;
    for (int i =1;i<=n;i++)
    {
        count = count * i;
    }
    return count;
}

int main()
{
    
    int n,result;
    cin>>n;
    result = fact(n);
    cout<<result;
    return 0;
}

```
