# Math

## Find the highest value of two numbers

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << max(5, 10) << endl;

    return 0;
}
```

Output:

```text
10
```

## Find the lowest value of two numbers

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << min(5, 10) << endl;

    return 0;
}
```

Output:

```text
5
```

## Use the cmath header file for other math functions

Code:

```cpp
#include <iostream>
#include <cmath>
using namespace std;

int main() {
    cout << sqrt(64) << "\n";
    cout << round(2.6) << "\n";
    cout << log(2) << "\n";

    return 0;
}
```

Output:

```text
8
3
0.693147
```