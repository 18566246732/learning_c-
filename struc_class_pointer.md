### Structure

structure is combination of different data types


### class
each class has a constructor which has the same name as the class name
```c++
class cow {
public:
  cow(string _name, int _age, unsigned char _purpose) {
    name = _name;
    age = _age;
    purpose = _purpose;
  }
private:
  string name;
  int age;
  unsigned char purpose;
}
```

### source and header file

how c++ files get executed:

source file -> assembly file -> object file

![img](https://user-images.githubusercontent.com/32592393/198836640-953f34ba-5fb5-473c-8b91-d978b464c4df.png)
- source file
your c++ code, these file are sent to the 1nd program known as the `compiler`

- assembly file
human readable version of the navite language of the target CPU, these files are sent to the 2nd programe known as the `assembler`

- object file
which are correlated pieces of your project, these file are sent to the 3rd program known as the `linker`

- make file
sometimes the compiler needs to interact with the command-line, which can be complicated, so the makeFile comes to rescue.


### pointers
pointers can save memory, you can create a class pointer, which can point to a class entity
```c++
// for example, if cow is a class
cow * my_cow = new cow(10, "sandy", meat);

// if you do not use pointer, it will create much more memory
cow my_cow(10, "sandy", meat);
```

if we write:
```c++
int a = 34;
int *ptr = &a;
```

then we have to understand the meaning of:
1. a
2. &a
3. ptr
4. \*ptr
5. &ptr

### reference

reference is not a object or a pointer, it has no memory address, therefore:
1. we can't create reference of an array.
2. there are no references to references.
  both references will point to the same object
3. there are no pointers to references.

#### difference between pointers and references
pointers are more powerful, references are more safe
![img](https://user-images.githubusercontent.com/32592393/199511839-bb58b3f5-e479-4ffc-a22c-dfcebde45961.png)
