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

### source and header file

how c++ files get executed:

source file -> assembly file -> object file
![Screen Shot 2022-10-29 at 22 21 52](https://user-images.githubusercontent.com/32592393/198836640-953f34ba-5fb5-473c-8b91-d978b464c4df.png)
