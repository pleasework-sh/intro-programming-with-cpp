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
Note the contents of this file. You will need to paste it into gedit later before you run it. 

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

Run the following commands:
```
cd <folder of your repository>

mkdir module1

cd module1

gedit helloworld.cpp
```

Save the file after pasting it into gedit.

```
g++ helloworld.cpp -o hello
chmod +x hello
./hello

git add .
git commit -m "first file"
git push origin main
```

Take a screenshot of the file running and submit it in a .docx or pdf file with a link to the file in your github repository. 