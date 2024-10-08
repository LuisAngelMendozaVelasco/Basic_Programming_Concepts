# Conditions

## The if statement

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    if(20 > 18) {
        cout << "20 is greater than 18!" << endl;
    }  

    return 0;
}
```

Output:

```text
20 is greater than 18!
```

## The else statement

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int time = 20;

    if(time < 18) {
        cout << "Good day!" << endl;
    } 
    else {
        cout << "Good evening!" << endl;
    }

    return 0;
}
```

Output:

```text
Good evening!
```

## The else if statement

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int time = 22;

    if(time < 10) {
        cout << "Good morning!" << endl;
    } 
    else if(time < 20) {
        cout << "Good day!" << endl;
    } 
    else {
        cout << "Good evening!" << endl;
    }

    return 0;
}
```

Output:

```text
Good evening!
```