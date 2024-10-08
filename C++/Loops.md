# Loops

## While loop

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 0;

    while(i < 5) {
        cout << i << "\n";
        i++;
    }

    return 0;
}
```

Output:

```text
0
1
2
3
4
```

## Do while loop

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 0;

    do {
        cout << i << "\n";
        i++;
    }
    while (i < 5);

    return 0;
}
```

Output:

```text
0
1
2
3
4
```

## For loop

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    for(int i = 0; i < 5; i++) {
        cout << i << "\n";
    }

    return 0;
}
```

Output:

```text
0
1
2
3
4
```

## Break a loop

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    for(int i = 0; i < 10; i++) {
        if(i == 4) {
            break;
        }
        cout << i << "\n";
    } 

    return 0;
}
```

Output:

```text
0
1
2
3
```

## Continue a loop

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    for(int i = 0; i < 10; i++) {
        if(i == 4) {
            continue;
        }
        cout << i << "\n";
    }   

    return 0;
}
```

Output:

```text
0
1
2
3
5
6
7
8
9
```