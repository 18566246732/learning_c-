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
