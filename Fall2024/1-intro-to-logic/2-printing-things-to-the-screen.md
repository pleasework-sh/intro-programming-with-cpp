# Printing things to the screen
Let's break down our first helloworld.cpp file.

```c++
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!";
    return 0;
}
```

What does each line mean? I'll break this down using **comments**. Using comments in programming is like adding annotations, or sticky notes, to your code. The **compiler** will IGNORE any comments you add to your code. But first, let's talk a little bit about syntax.

Every programming language has a certain **syntax**, or rules of the language. Think of syntax like you would grammar. To write in proper English, you have to capitalize the beginning of sentences, and end them with a symbol like a period (.), question mark (?), or exclamation point! Additionally, in proper English, when you're describing a person, place, or thing, the adjective has to come before that noun. I would write something like "the red dog" as opposed to "the dog red" (which would be valid in other languages if you translated them literally).

Let's take a look at the classic "Hello, world!" program in different languages.

**C++**
```c++
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!";
    return 0;
}
```

**Java**
```java
public class HelloWorld {

    public static void main(String[] args) {
        System.out.println("Hello, world");
    }

}
```
**Python**
```python
print("Hello, world!")
```

All of these programs do the same thing, that is print "Hello, world!" to the screen when you run them. Note how these languages differ, yet if you examine the files carefully, you can start to understand what they mean. 

This course is meant to help you learn the **fundamentals** of programming that you can take with you to apply in any language, not just C++. We are simply using C++ as a starting point.

Here is our helloworld.cpp file, now with comments. Comments in C++ are denoted with either either two backslashes `//` (single line) or a backslash asterisk `/*` and closed off with an asterisk backslash `*/`.

**helloworld.cpp, now with comments**
```c++
// this is a single line comment
// this includes the iostream library, which contains
// what we need for input / output
#include <iostream>
// namespaces in C++ are used to organize code
// we aren't going too in depth about what namespaces are
// for now, just keep this in your code as a habit
using namespace std;

/* 
This is a multiline comment. 
Here, we define our main() function. Typically
languages will have a main() function that runs
upon program execution.
*/
int main() {

    // this is the line that prints "Hello, world!" to our screen.
    cout << "Hello, world!";

    // this is the program exit code.
    // programs may have different exit codes to denote
    // different results, errors, etc...
    // for our purposes, upon successful execution
    // our program returns 0
    return 0;
}
```

## Assignment 1: Comments
> [!TIP]  
> Take the file below, add your own comments (whatever you would like). Try running the program and see what happens. Name it 1-comments.cpp

```c++
// write your comments wherever you want.
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!";
    return 0;
}
```

As a reminder, this is how you compile and run programs.
```
gedit 1-comments.cpp
# ... make your edits and save them in gedit

g++ 1-comments.cpp -o comments
chmod +x comments
./comments
```

Craft a word document with a link to your code and a screenshot of the code running. What is different about program execution? 

If you said nothing, that's right! Comments are meant to be ignored, but are helpful for us programmers to understand what is going on in our code. For our super simple hello world programs, comments might not be necessary, but they become more useful as what we write becomes more complex.