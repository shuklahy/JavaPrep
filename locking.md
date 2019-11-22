## Locking in Java

Locks in Java is acquired at 2 levels
* Object level locks
* Class level locks

### Object level locks
In case of object level locks, only one thread can enter the `synchronized` block for a given object. 
Eg. Lets say you have a object hello1 of class Hello and a synchronized method called sayHello, if some threads say 1, 2 and 3
all are calling 
- 1 -> hello1.sayHello()
- 2 -> hello1.sayHello()
- 3 -> hello1.sayHello()

so only one thread will be able to call hello1.sayHello() at any given moment of time

### Class level locks
 In case of class level locks since locks are acquired at level class only one thread can enter class synchronized blocks.
 so say you have 100 instance
