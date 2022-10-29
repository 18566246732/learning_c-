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
``

