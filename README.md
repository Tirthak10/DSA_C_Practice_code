# DSA_C_Practice_code
# Simple C++ Input/Output Program

This is a basic C++ program that demonstrates how to take input from the user and display it using `cin` and `cout`.

## 💻 Code

```cpp
// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;

int main() {
    int x , y;
    cin >> x >> y;
    cout << "The value of x : " << x << " And y : " << y;
    return 0;
}

Example input:
10 20
Example output:
The value of x : 10 And y : 20

```
# Simple C++ Program: Demonstration of `float` and `double` Data Types

This program is a simple example to show how `float` and `double` data types work in C++.

## 💻 Code

```cpp
// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;

int main() {
   // float, double datatypes
   float x = 5.6;
   double y = 6;
   cout << "Value of Y is : " << y;
   return 0;
}

Value of Y is :6
```
# 🧾 C++ Program: Using `string` and `getline`

This program demonstrates how to take string input from the user using `cin` and output it using `cout`. While it uses basic `cin`, it's a foundational step before using more advanced input functions like `getline()`.

---

## 💻 Code

```cpp
// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;

int main() {
    // String and getline
    string s1, s2;
    cin >> s1 >> s2;
    cout << s1 << " " << s2;
    return 0;
}
```
This program demonstrates how to take an entire line of input using `getline()` in C++. This is useful when you want to capture a sentence or string containing spaces.
```cpp
#include <iostream>
using namespace std;

int main() {
    // String and getline 
    // In case you want to take everything together in a string, use getline.
    string str;
    getline(cin, str);
    cout << str;
    return 0;
}

Input  : Cybersecurity is a fascinating field!
Output : Cybersecurity is a fascinating field!
```
# 🧾 C++ Program: Single Character Input with `char`

This C++ program takes a single character as input from the user using `cin` and prints it back using `cout`.

## 💻 Code

```cpp
#include <iostream>
using namespace std;

int main() {
    // Using char for single character input
    char str;
    cin >> str;
    cout << str;
    return 0;
}
Input : T
Output : T
```
