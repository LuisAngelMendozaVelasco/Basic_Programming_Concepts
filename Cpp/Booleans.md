# Booleans

## Boolean values

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    bool isCodingFun = true;
    bool isFishTasty = false;

    cout << isCodingFun << "\n";
    cout << isFishTasty << endl;

    return 0;
}
```

Output:

```text
1
0
```

## Compare two values

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << (10 > 9) << endl;

    return 0;
}
```

Output:

```text
1
```

## Compare two variables

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x = 10;
    int y = 9;

    cout << (x > y) << endl;

    return 0;
}
```

Output:

```text
1
```