# Inheritance ![Inheritance](https://img.shields.io/badge/Inheritance-purple)
## Founder : Rahimjonov Otabek
## HomeWork 
### *Protected*
**Bu `class` ichidagi ma'lumotni hamma `class` lar ishlatmasligi uchun cheklaydi, lekin ayrim `class` larga ruxsat beradi** ![Protected](https://img.shields.io/badge/Protected-yellow)
```java
    public class Main{
        Protected String name;

        public Main(String name) {
            this.name = name;
        }
    }
```
***
### *Extends*
**Yana bitta `class` boshqa `class`ning xususiyati va methodlari o'zlashtiradi** ![Extends](https://img.shields.io/badge/Extends-red)
```java
public class Dog extends Main {
  public Dog (String name ) {
      super(name);
  }
    public static void main(String [] args){
       Dog dog = new Dog();
    }
}
```
**Super**
