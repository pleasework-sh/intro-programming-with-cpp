# Using gedit
We will be using the text editor `gedit` to edit and run our code.

In the terminal run 
```
gedit insert_desired_file_name
```
gedit will open. From here, you can start messing around, editing the file and saving it.

If gedit is NOT installed (if you get an error), run the following commands:

```
sudo apt-get update
sudo apt-get install gedit
```

You may be prompted to enter your user password.

# Contents of the helloworld.cpp file
Note the contents of this file. You will need to paste it into gedit later before you run and compile the file.

You can copy and paste it directly from below. 
```c++
#include <iostream>
using namespace std;

int main() {
    cout << "Hello, world!";
    return 0;
}
```

# Running your first cpp file
Now that you've finished the long arduous process of setting up your development environment, you are finally ready to run your first file.

If you are getting an error when trying to run g++ run the following commands:
```
sudo apt-get update
sudo apt-get install g++
```
Run the following commands in the terminal.
```
cd <folder of your repository>

mkdir module1

cd module1

gedit helloworld.cpp
```
Once you see the file open in your text editor, go ahead and copy the file contents above from the section "Contents of the helloworld.cpp file".

Save the file after pasting it into gedit. Close the file.


Note that you need to close the helloworld.cpp file. Then you need to open your terminal and run the following commands.
```
g++ helloworld.cpp -o hello
chmod +x hello
./hello

git add .
git commit -m "first file"
git push origin main
```

Take a screenshot of the file running and submit it in a .docx or pdf file with a link to the file in your github repository. 
