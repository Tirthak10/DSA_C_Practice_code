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
# 🚀 C++ Basics – Input, Strings, and If-Else

---

## 📥 0) Taking Input in C++

```cpp
cin >> x; // Taking user input in x variable
```

---

## 🧵 1) Input String Example

We want to take the input string `"Hey Tirthak"`, so we write:

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    string s;
    cin >> s;
    cout << s;
    return 0;
}
```

### 🔎 Output:
```
Hey
```

It didn't take the whole string `"Hey Tirthak"`.

---

## ✌️ 2) Taking Input Using Two Strings

```cpp
int main() {
    string s1;
    string s2;

    cin >> s1 >> s2;
    cout << s1 << " " << s2;
    return 0;
}
```

### ❗ Explanation:
If you use `cin` with `string`, it only picks up input **before the space**. After the space, it's treated as new input, so you have to use `cin` again.

---

## 📜 3) Taking Full Line Input with `getline()`

To take everything together in a string (including spaces), we use `getline()`:

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    string str;
    getline(cin, str); // Takes entire input line including spaces
    cout << str;
    return 0;
}
```

### 🧾 Output:
```
Hey Tirthak
```

---

### ℹ️ Example:

**Input:**
```
Hey Tirthak you're so Cool  // Only this line gets picked up
Hey Raj 
```

➡️ `getline()` captures the entire string **till the line break**.

---

## 🔢 4) Choosing Numeric Data Types

Let's say you want to store the number `10`. It can be stored in:

- `int`
- `long`
- `long long`
- `float`
- `double`

But why not always use `long long` or `double`?

Because **memory usage matters**. Each data type takes a different amount of memory. Use the **smallest required type**.

### 📏 Rule of Thumb:

| Data Type   | Approximate Range       |
|-------------|--------------------------|
| `int`       | -10⁹ to 10⁹             |
| `long`      | -10¹² to 10¹²           |
| `long long` | -10¹⁸ to 10¹⁸           |

Whenever the number exceeds the typical range (e.g., `10^13`), use `long long`.

---

## 🔁 IF-ELSE Statement

---

### ✅ Program: Check if age is adult

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int age;
    cin >> age;

    if(age >= 18) {
        cout << "You are an adult";
    } else {
        cout << "You are not an adult";
    }

    return 0;
}
```

**Input:** `14`  
**Output:** `You are not an adult`

**Input:** `21`  
**Output:** `You are an adult`

---

### ✨ Modified with `else if`

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    int age;
    cin >> age;

    if(age >= 18) {
        cout << "You are an adult";
    } else if(age < 18) {
        cout << "You are not an adult";
    }

    return 0;
}
```

> This version uses `else if` to further define the alternative case.

---

### ❓ Is `else` mandatory?

**No**, it's optional.  
If no `else` is present and the `if` condition fails, the program simply skips over the block.

---

## ✅ Summary of Learnings

- Use `cin` for basic inputs.
- Use `getline()` to capture entire lines with spaces.
- Choose numeric data types based on size and memory efficiency.
- `if`, `else if`, and `else` help implement logical flow.

---


