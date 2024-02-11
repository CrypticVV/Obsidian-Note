面向对象编程(OOP)之所以被认为是一种高级语言的重要特征,主要因为它符合人类思维方式,并且提高了代码的复用性、维护性和扩展性。具体优点包括:

1. 易于理解和组织代码:OOP通过使用类和对象来组织代码,类似我们人类对世界的认知方式。这让程序更加直观易懂。
2. 提高复用性:OOP通过类和继承机制,可以方便地复用已有代码。子类继承父类后,可以直接使用父类的属性和方法。
3. 提高维护性:OOP通过对象和数据封装,可以在不影响其他代码的情况下更新程序。这减少了代码之间不必要的依赖。
4. 提高扩展性:OOP通过继承和多态,可以轻易地对程序进行扩展。如果要添加新的特性,只需要基于现有类创建子类即可实现。
5. 为大型项目提供结构化方法:OOP通过类的划分,可以使大项目中的代码组织有明确结构。也方便多人协作开发。

所以简而言之,OOP更符合人类思维方式,让代码易于理解、连接和扩展,非常适合组织和维护大型项目。这就是它被广泛应用的根本原因之一。对新手来说,这种编程范式也更易于上手。

***Without OOP***
```python
struct AnimalProperties {
  string name;
  string species;
  int age;
}

struct DogProperties {
  string name; 
  string species = "Dog";
  int age;
  string breed; 
}

void foo(AnimalProperties a) {
  printf("Name: %s, Species: %s, Age: %d", a.name, a.species, a.age); 
}

int main() {

  AnimalProperties a1; 
  a1.name = "Mikey";
  a1.species = "Monkey";
  a1.age = 3;

  DogProperties d1;
  d1.name = "Rocky";  
  d1.age = 4; 
  d1.breed = "German Shephard";

  foo(a1);
  foo(d1);

}
```

***With OOP***
```python
class Animal {
  protected:
    string name;
    string species; 
    int age;

  public:
    void printInfo() {
      printf("Name: %s, Species: %s, Age: %d", name, species, age); 
    }
}

class Dog extends Animal {
  private:
    string breed;
  
  public:
    void printDogInfo() {
      printInfo(); 
      printf(", Breed: %s", breed); 
    }
}


int main() {

  Animal a1 = Animal("Mikey", "Monkey", 3);  
  Dog d1 = Dog("Rocky", 4, "German Shephard");

  a1.printInfo(); 
  d1.printDogInfo();

}
```

