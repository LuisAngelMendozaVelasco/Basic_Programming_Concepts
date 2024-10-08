# Data Types

## A demonstration of different data types

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;
 
int main () {
    // Creating variables
    int myNum = 5;               // Integer (whole number)
    float myFloatNum = 5.99;     // Floating point number
    double myDoubleNum = 9.98;   // Floating point number
    char myLetter = 'D';         // Character
    bool myBoolean = true;       // Boolean
    string myString = "Hello";   // String

    // Print variable values
    cout << "int: " << myNum << "\n";
    cout << "float: " << myFloatNum << "\n";
    cout << "double: " << myDoubleNum << "\n";
    cout << "char: " << myLetter << "\n";
    cout << "bool: " << myBoolean << "\n";
    cout << "string: " << myString << "\n";

    return 0;
}
```

Output:

```text
int: 5
float: 5.99
double: 9.98
char: D
bool: 1
string: Hello
```

## Create an int type

Code:

```cpp
#include <iostream>
using namespace std;
 
int main () {
    int myNum = 1000;

    cout << myNum << endl;
    cout << "Size of int: " << sizeof(int) << " bytes" << endl;

    return 0;
}
```

Output:

```text
1000
Size of int: 4 bytes
```

## Create a float type

Code:

```cpp
#include <iostream>
using namespace std;
 
int main () {
    float myNum = 5.75;

    cout << myNum << endl;
    cout << "Size of float: " << sizeof(float) << " bytes" << endl;

    return 0;
}
```

Output:

```text
5.75
Size of float: 4 bytes
```

## Create a double type

Code:

```cpp
#include <iostream>
using namespace std;
 
int main () {
    double myNum = 19.99;

    cout << myNum << endl;
    cout << "Size of double: " << sizeof(double) << " bytes" << endl;

    return 0;
}
```

Output:

```text
19.99
Size of double: 8 bytes
```

## Create boolean types

Code:

```cpp
#include <iostream>
using namespace std;

int main() {
    bool isCodingFun = true;
    bool isFishTasty = false;

    cout << isCodingFun << "\n";
    cout << isFishTasty << endl;
    cout << "Size of bool: " << sizeof(bool) << " bytes" << endl;

    return 0;
}
```

Output:

```text
1
0
Size of bool: 1 bytes
```

## Create a char type

Code:

```cpp
#include <iostream>
using namespace std;
 
int main () {
    char myGrade = 'B';

    cout << myGrade << endl;
    cout << "Size of char: " << sizeof(char) << " bytes" << endl;

    return 0;
}
```

Output:

```text
B
Size of char: 1 bytes
```

## Create a string type

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string greeting = "Hello";

    cout << greeting << endl;
    cout << "Size of string: " << sizeof(string) << " bytes" << endl;

    return 0;
}
```

Output:

```text
Hello
Size of string: 32 bytes
```