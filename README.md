# Code-I-wrote-as-an-undergraduate3
For 100,000 lines of code
//初识搜索二叉树————函数递归————走方格//
```
#include<iostream>
using namespace std;
void dfs(int x, int y);
int n, m;
int ans;
int main()
{
    cin >> n >> m;
    dfs(0, 0);
    cout << ans;

    return 0;
}

void dfs(int x, int y)
{
    if (x == n && y == m)
    {
        ans++;
    }
    else {
        if (x < n)
        {
            dfs(x + 1, y);
        }

        if (y < m)
        {
            dfs(x, y + 1);
        }
    }
}
```
