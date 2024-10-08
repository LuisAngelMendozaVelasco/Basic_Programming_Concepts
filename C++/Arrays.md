# Arrays

## Create and access an array

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};

    cout << cars[0] << endl;

    return 0;
}
```

Output:

```text
Volvo
```

## Change an array element

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};

    cars[0] = "Opel";
    cout << cars[0] << endl;

    return 0;
}
```

Output:

```text
Opel
```

## Loop through an array

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string cars[4] = {"Volvo", "BMW", "Ford", "Mazda"};

    for(int i = 0; i < 4; i++) {
        cout << cars[i] << "\n";
    }

    return 0;
}
```

Output:

```text
Volvo
BMW
Ford
Mazda
```

## Get the size/length of an array

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    int myNumbers[5] = {10, 20, 30, 40, 50};

    cout << sizeof(myNumbers) << " bytes" << endl;

    return 0;
}
```

Output:

```text
20 bytes
```

## Multidimensional arrays

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    string letters[2][4] = {{"A", "B", "C", "D"},
                            {"E", "F", "G", "H"}};

    cout << letters[0][2] << endl;

    return 0;
}
```

Output:

```text
C
```