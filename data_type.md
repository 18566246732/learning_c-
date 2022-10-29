### variable and basic type

- pointer
  1. pointer must be initialized with a actual value or empty value such as nullptr/0, or it will cause a bug
  2. pointer can change the one to point to
  3. pointer can point to another pointer (**)
  
- void* pointer
  1. can point to the address where the value is any type.
  2. can't get the object of the address
  3. mainly used as function I/O

- reference
  1. reference must be initialized when defined, and it will create a bind with the original object
  2. it can't change the reference
  3. reference can't refer to another reference, but can refer to a pointer(because pointer is a object).
  `int *&r = p;`
  
- declare multiple type using one instruction
 ```c++
 int i = 1024, *p = &i, &r = 1;
 // this means *p1, and p2 is not a pointer !!!
 int* p1, p2;
 ```
 
- const
  1. const only works on the logical side, it doesn't work on the address side.
  ```c++
  int i = 42;
  const int &r = i;
  // the value of "r" will change if we change the value of i
  i = 43;
  ```
  2. pointer to const vs const pointer
  ```c++
  int errNumb = 0;
  int *const curErr = errNumb;
  ```
  3. top-level and low-level const
  if `const` is in the right of `*`, then it's a top-level(the pointer is a const), otherwise it's a low-level(the pointer of value is a const)
  
  4. const assignment
  non-const value can convert to const value, const value can't convert to non-const.
  
### Type reference with auto
 
```c++
#include <iostream>
#include <typeinfo>

using namespace std;

auto a = 8;
auto b = 12345678901;
auto c = 3.14f;
auto d = 3.14;
auto f = 'd';

int main(int argc, char const *argv[])
{
    cout << typeid(a).name() << endl; // i(int)
    cout << typeid(b).name() << endl; // l(long)
    cout << typeid(c).name() << endl; // f(float)
    cout << typeid(d).name() << endl; // d(double)
    cout << typeid(f).name() << endl; // f(char)
    return 0;
}
```
 
### preprocessor directives
directives are not end with semicolon.
- include
  ```c++
  #include <xxx>
  ```

- define
  used to define some symbol, there symbol are called `macro`
  ```c++
  define CAPACITY 5000
  ```
  
  used for debugging purpose, first we set up the following test code
  ```c++
  #ifdef DEBUG
  // do something
  #endif
  ```
  then we open the debug by adding definition for the `DEBUG`
  ```c++
  #define DEBUG
  ```

  
  
  

### constants
the use of constants is sometimes discouraged

### data type
the default type of integer is `int`

the default type of decimal is `double`

