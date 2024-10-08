# Switch

## The switch statement

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int day = 4;

    switch(day) {
        case 1:
            cout << "Monday" << endl;
            break;
        case 2:
            cout << "Tuesday" << endl;
            break;
        case 3:
            cout << "Wednesday" << endl;
            break;
        case 4:
            cout << "Thursday" << endl;
            break;
        case 5:
            cout << "Friday" << endl;
            break;
        case 6:
            cout << "Saturday" << endl;
            break;
        case 7:
            cout << "Sunday" << endl;
            break;
    }

    return 0;
}
```

Output:

```text
Thursday
```

## The switch statement with a default keyword

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int day = 4;

    switch(day) {
        case 6:
            cout << "Today is Saturday!" << endl;
            break;
        case 7:
            cout << "Today is Sunday!" << endl;
            break;
        default:
            cout << "Looking forward to the Weekend!" << endl;
    }

    return 0;
}
```

Output:

```text
Looking forward to the Weekend!
```