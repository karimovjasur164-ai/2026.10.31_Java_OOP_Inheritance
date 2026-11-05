# ☕ Java Developer: Inheritance ![Inheritance](https://img.shields.io/badge/Inheritance-purple)

**Inheritance (Merosxo'rlik)** — OOP (Obyektga yo'naltirilgan dasturlash) ning asosiy prinsiplaridan biri bo'lib, bir klassning xususiyatlari (fields) va metodlarini ikkinchi klassga o'tkazish imkonini beradi.

---

###  Protected modifikatori ![Protected](https://img.shields.io/badge/Protected-yellow)
Bu klass ichidagi ma'lumotlarni hammadan cheklaydi, lekin undan meros olgan voris klasslarga va o'sha paket (package) ichidagi boshqa klasslarga ishlatish uchun ruxsat beradi.

```java
public class Main {
    protected String name;

    public Main(String name) {
        this.name = name;
    }
}
```

---

###  Extends kalit so'zi ![Extends](https://img.shields.io/badge/Extends-blue)
Bitta klass boshqa klassning xususiyatlari va metodlarini o'zlashtirishi (meros olishi) uchun `extends` kalit so'zidan foydalaniladi.

```java
public class Dog extends Main {
    public Dog(String name) {
        super(name); // Ota klass konstruktorini chaqirish
    }

    public static void main(String[] args) {
        Dog dog = new Dog("Tuzik");
    }
}
```

---

###  Super() metodi ![Super()](https://img.shields.io/badge/Super()-red)
Java-da `super()` metodi ota (parent) klassning konstruktorini voris (child) klass ichidan chaqirish uchun ishlatiladi. Voris klass (`Dog`) ota klass (`Animal`) konstruktoriga kerakli parametrlarni uzatadi va uni ishga tushiradi.

```java
public class Animal {
    protected String name;
    protected int age;

    public Animal(String name, int age) {
        this.name = name;
        this.age = age;
    }
}

class Dog extends Animal {
    public Dog(String name, int age) {
        super(name, age); // Ota klass (Animal) konstruktorini ishga tushirish
    }

    public static void main(String[] args) {
        Dog dog = new Dog("Rex", 3);
    }
}
```
