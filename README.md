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
**Yana bitta `class` boshqa `class`ning xususiyati va methodlari o'zlashtiradi** ![Extends](https://img.shields.io/badge/Extends-blue)
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
***
### *Super*  
**Java - da `Super()` - ota `class` konsturktorini chaqirish uchun ishlatiladi yani Voris `extends` `(dog)` ota `class` esa `(Animal)` - dan meros oladi `super()` esa ota `class` konsturktorini ishga tushuradi** ![Super()](https://img.shields.io/badge/Super()-red)
```java
public class Animal {
   protected String name;
   protevted int age;

   public Animal(String name, int age) {
       this.name = name;
       this.age = age;
   }
}
class Dog extends Animal {
   public Dog (String name, int age){
      super(name, age);
   }
   public static void main(String [] args){
     Dog dog = new Dog();
   }
```
***
