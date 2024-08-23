# Experiment 2
## Program 1
### Aim:
To display the size of each primitive data type in C++.

### Software Used:
Visual Studio Code

## Theory:
In C++, primitive data types are the basic types that come built into the language. They include:
int: For storing integers.
float: For storing single-precision floating-point numbers.
double: For storing double-precision floating-point numbers.
char: For storing single characters.
bool: For storing boolean values (true or false).
The sizeof operator in C++ helps determine the size of these data types, variables, and constants at compile time.

### Program Code:
``` javascript
g#include <iostream>
using namespace std;
int main(){
    cout<< "Size of intergers is "<< sizeof(int)<< " bytes"<< endl;
    cout<< "Size of float is "<< sizeof(float)<< " bytes"<< endl;
    cout<< "Size of strings is "<< sizeof(string)<< " bytes"<< endl;
    cout<< "Size of character is "<< sizeof(char)<< " bytes"<< endl;
    cout<< "Size of double is "<< sizeof(double)<< " bytes"<< endl;
    cout<< "Size of long is "<< sizeof(long)<< " bytes"<< endl;
    cout<< "Size of boolean is "<< sizeof(bool)<< " bytes"<< endl;
    return 0;
}
```
### Output:
![image](https://github.com/user-attachments/assets/5c8f7956-dd38-4e84-80a0-e573ed8eda51)

### Conclusion:
We explored and displayed the sizes of different primitive data types in C++.

## Program 2
### Aim:
To demonstrate the use of storage classes in C++.

### Software Used:
Visual Studio Code

## Theory:
Storage classes in C++ determine the visibility and lifetime of variables and functions:

auto: Automatically deduces the type of a variable. It lets the compiler figure out the type based on the assigned value.
register: Suggests storing the variable in a CPU register for quicker access. This is just a suggestion, not a command.
static: Limits the scope of a variable to the file, function, or block where it's defined but keeps its value between function calls.
extern: Indicates that a variable or function is defined in another file or later in the same file, allowing for sharing across files.
Output:
The program will demonstrate the effects and behaviors of different storage classes.

### Program code:
``` javascript
#include <iostream>
using namespace std;
void staticExample(){
    //int z=0;
    static int z=0;
    z++;
    cout<< "The value of z is: "<<z<<endl;
}

int main(){
    staticExample();
    staticExample();
    staticExample();    
    return 0;
}
```

### Output:
![image](https://github.com/user-attachments/assets/038bcc12-e1aa-4ee1-8eb4-6b540eeb5de9)


### Conclusion:
We learned about storage classes in C++ and how they affect variable scope and lifetime.
