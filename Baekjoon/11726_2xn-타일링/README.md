# 2xn 타일링

```cpp
#include <iostream>
using namespace std;

int main()
{
    int n;
    int res[1000] = {1, 2, };
    cin >> n;

    for(int i=2; i<n; i++){
        res[i] = (res[i-1]+res[i-2])%10007;
    }
    cout << res[n-1];
    return 0;
}
```
