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

## ✅ Multi-line Comments

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {

    /*
    you can just write 
    this symbol and write anything 
    and make a para also if u want 
    till u end it with this symbol
    */

}
```

---

## 📌IF Else Statements

Question: Grading System

### Code:

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
A school has following rules for grading system :
a. Below 25 - F
b. 25 to 44 - E
c. 45 to 49 - D
d. 50 to 59 - C
e. 60 to 79 - B
f. 80 to 100 - A
Ask user to enter marks and print the corresponding grade.
*/

int main() {
    int marks;
    cin >> marks;
    if(marks < 25){
        cout << "F";
    }
    else if(marks >= 25 && marks <= 44){
        cout << "E";
    }
    else if(marks >= 45 && marks <= 49){
        cout << "D";
    }
    else if(marks >= 50 && marks <= 59){
        cout << "C";
    }
    else if(marks >= 60 && marks <= 79){
        cout << "B";
    }
    else if(marks >= 80 && marks <= 100){
        cout << "A";
    }
    return 0;
}
```

### Example:

```
Input  : 21
Output : F

Input  : 72
Output : B
```

---

## 🔁 Trimmed Version of Grading System

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
A school has following rules for grading system :
a. Below 25 - F
b. 25 to 44 - E
c. 45 to 49 - D
d. 50 to 59 - C
e. 60 to 79 - B
f. 80 to 100 - A
Ask user to enter marks and print the corresponding grade.
*/

int main() {
    int marks;
    cin >> marks;
    if(marks < 25){
        cout << "F";
    }
    else if(marks <= 44){
        cout << "E";
    }
    else if(marks <= 49){
        cout << "D";
    }
    else if(marks <= 59){
        cout << "C";
    }
    else if(marks <= 79){
        cout << "B";
    }
    else if(marks <= 100){
        cout << "A";
    }
    return 0;
}
```

---

## 🔎 NESTED If-Else Question

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
Take the age from the user and then decide accordingly 
1. If age < 18;
print -> not eligible for the job

2. If age >= 18;
print -> "eligible for job"

3. If age >= 55 and age <= 57;
print -> "eligible for job, but retirement soon."

4. If age > 57
print -> "retirement time"
*/

int main() {
    int age;
    cin >> age;
    if(age < 18){
        cout << "Not eligible for the job";
    }
    else if(age <= 55){
        cout << "eligible for the job";
    }
    else if(age <= 57){
        cout << "eligible for the job, but retirement soon";
    }
    else{ 
        cout << "Retirement time";
    }
    return 0;
}
```

### 🔸 Brief Description:
This code takes a user's age and uses a sequence of if-else conditions to check and print the eligibility for a job. It first checks if the person is under 18, then between 18 and 55, between 55 and 57 (indicating nearing retirement), and finally checks if the person is above 57 for retirement.

---

## 🧠 Nested IF (Alternative Version)

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
Take the age from the user and then decide accordingly 
1. If age < 18;
print -> not eligible for the job

2. If age >= 18;
print -> "eligible for job"

3. If age >= 55 and age <= 57;
print -> "eligible for job, but retirement soon."

4. If age > 57
print -> "retirement time"
*/

int main() {
    int age;
    cin >> age;
    if(age < 18){
        cout << "Not eligible for the job";
    }
    else if(age <= 57){
        cout << "eligible for the job";
        if(age >= 55){
            cout << ", but retirement soon";
        }
    }
    else{ 
        cout << "Retirement time";
    }
    return 0;
}
```

### 🔸 Brief Description:
This code uses a nested `if` inside the outer `else if(age <= 57)` block. This allows combining the general eligibility check (`age <= 57`) with a special case for nearing retirement (`age >= 55`)—producing cleaner and slightly more efficient code than checking each age range separately.

# 🚦 Switch Statements in C++

Switch statements are similar to `if-else` constructs but are typically used less often. Still, it's useful to understand them.

We use `switch` when we want to take decisions based on the value of a variable. In this example, we demonstrate how to print the name of the day based on a number from 1 to 7.

---

## 🧠 Concept Overview

You write `switch(variable)` and define cases for each expected value.

---

## ❓ Problem Statement

**Take the day number and print the corresponding day.**

| Input | Output  |
|-------|---------|
| 1     | Monday  |
| 2     | Tuesday |
| ...   | ...     |
| 7     | Sunday  |

---

## ⚠️ Incorrect Code: Without `break`

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
Take the day no and print the corresponding day
for 1 print Monday,
for 2 print Tuesday and so on for 7 print Sunday
*/

int main() {
    int day;
    cin >> day;

    switch (day) {
        case 1 :
            cout << "Monday";
        case 2 :
            cout << "Tuesday";
        case 3 :
            cout << "Wednesday";
        case 4 :
            cout << "Thursday";
        case 5 :
            cout << "Friday";
        case 6 :
            cout << "Saturday";
        case 7 :
            cout << "Sunday";    
        return 0;
    }
}
```

### 🔎 Input: `5`  
**Output:** `FridaySaturdaySunday`

As you can see, it starts at case 5 and executes all the statements after that. This is because there's **no `break`** statement to stop the execution after the match.

---

## ✅ Corrected Code: With `break`

To prevent the fall-through behavior seen above, we add `break` after every case.

```cpp
#include <bits/stdc++.h>
using namespace std;

/*
Take the day no and print the corresponding day
for 1 print Monday,
for 2 print Tuesday and so on for 7 print Sunday
*/

int main() {
    int day;
    cin >> day;

    switch (day) {
        case 1 :
            cout << "Monday";
            break;
        case 2 :
            cout << "Tuesday";
            break;
        case 3 :
            cout << "Wednesday";
            break;
        case 4 :
            cout << "Thursday";
            break;
        case 5 :
            cout << "Friday";
            break;
        case 6 :
            cout << "Saturday";
            break;
        case 7 :
            cout << "Sunday"; 
            break;
        default:
            cout << "Invalid";  
    }
    cout << " Check ";  
    return 0;
}
```

---

### ✅ Input: `5`  
**Output:** `Friday Check`

### ✅ Input: `19`  
**Output:** `Invalid Check`

---

## 📝 Explanation

- The `break` statement stops further execution inside the switch block.
- Without `break`, execution "falls through" to the next case.
- The `default` case is used when the input does not match any of the defined cases.

This version correctly handles the logic by isolating each case and terminating it properly, preventing unintended execution of subsequent cases.

---

Happy coding! 🚀
