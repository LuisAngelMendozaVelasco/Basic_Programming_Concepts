# Strings

## Create a string

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string greeting = "Hello!";

    cout << greeting << endl;

    return 0;
}
```

Output:

```text
Hello!
```

## String concatenation

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;
 
int main() {
    string firstName = "Luis ";
    string lastName = "Mendoza";
    string fullName = firstName + lastName;

    cout << fullName << endl;

    return 0;
}
```

Output:

```text
Luis Mendoza
```

## String length

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";

    cout << "The length of the txt string is: " << txt.length() << endl;

    return 0;
}
```

Output:

```text
The length of the txt string is: 26
```

## Access string characters

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string myString = "Hello";

    cout << myString[0] << endl;

    return 0;
}
```

Output:

```text
H
```

## Change string characters

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string myString = "Hello";

    myString[0] = 'J';
    cout << myString << endl;

    return 0;
}
```

Output:

```text
Jello
```

## User input strings

Code:

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string fullName;

    cout << "Type your full name: ";
    getline(cin, fullName);
    cout << "Your name is: " << fullName << endl;

    return 0;
}
```

Output:

```text
Type your full name: Luis Mendoza
Your name is: Luis Mendoza
```