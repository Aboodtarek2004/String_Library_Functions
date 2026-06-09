# String Library Functions 🧵

A simple C++ string utility library that provides common string operations using a custom `clsString` class.

This project is useful for practicing C++ classes, static functions, object methods, string manipulation, vectors, and basic text processing.

## Features ✨

* Get string length
* Count words
* Convert the first letter of each word to uppercase
* Convert the first letter of each word to lowercase
* Convert the whole string to uppercase
* Convert the whole string to lowercase
* Invert letter case
* Count capital letters
* Count small letters
* Count a specific letter
* Count vowels
* Split a string by delimiter
* Trim spaces from the left, right, or both sides
* Join strings from an array or vector
* Reverse words in a string
* Replace words with optional case sensitivity
* Remove punctuation marks

## Project Structure 📁

```text
String_Library_Functions/
│
├── String_Class/
│   ├── String_Class.cpp
│   ├── String_Library.h
│   ├── clsString.cpp
│   └── String_Class.vcxproj
│
└── String_Class.slnx
```

## Requirements 🛠️

* C++ compiler
* Visual Studio recommended
* Basic knowledge of C++ classes and strings

## How to Run 🚀

1. Clone the repository:

```bash
git clone https://github.com/Aboodtarek2004/String_Library_Functions.git
```

2. Open the solution/project in Visual Studio.

3. Build and run the project.

## Example Usage 💻

```cpp
#include <iostream>
#include "String_Library.h"

using namespace std;

int main()
{
    clsString text("hello world from c++");

    cout << "Original: " << text.Value << endl;

    text.UpperFirstLetterOfEachWord();
    cout << "Capitalized: " << text.Value << endl;

    cout << "Words count: " << text.CountWords() << endl;
    cout << "Length: " << text.Length() << endl;
    cout << "Vowels: " << text.CountVowels() << endl;

    return 0;
}
```

## Example Output 📌

```text
Original: hello world from c++
Capitalized: Hello World From C++
Words count: 4
Length: 20
Vowels: 5
```

## Main Class 🧱

The main class in this project is:

```cpp
class clsString
```

It supports both:

* Static functions that work directly on a given string
* Object functions that update or read the current object value

Example using a static function:

```cpp
clsString::CountWords("Hello world");
```

Example using an object:

```cpp
clsString text("Hello world");
text.CountWords();
```

## Purpose 🎯

This project was created as a practice project to improve C++ programming skills, especially:

* Object-Oriented Programming
* String handling
* Static methods
* Vectors
* Text processing logic

## Author 👨‍💻

Created by Abood Tarek.
