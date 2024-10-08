# User Input

## Input a number and print the result

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x;

    cout << "Type a number: "; // Type a number and press enter
    cin >> x; // Get user input from the keyboard
    cout << "Your number is: " << x << endl;

    return 0;
}
```

Output:

```text
Type a number: 1
Your number is: 1
```

## Input two numbers and print the sum

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int x, y;
    int sum;

    cout << "Type a number: ";
    cin >> x;
    cout << "Type another number: ";
    cin >> y;

    sum = x + y;
    cout << "\nSum is: " << sum << endl;

    return 0;
}
```

Output:

```text
Type a number: 1
Type another number: 2

Sum is: 3
```