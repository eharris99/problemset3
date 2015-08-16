###Inheritance is when you create a parent class (like Person or Shape) and then create multiple child classes that inherit methods from the parent.

### The child class (like its parent) is created by going File-> New -> File -> Cocoa Touch Class and then naming it, and choosing to make it a subclass. The first class has to be a subclass of NSObject. After that new classes can be subclasses of the object created by the program, like Person or Shape.

### The child can override the parent by putting a new implementation inside an old method name. Or it can continue to use the parent's method by using the super class

### One tricky thing is to always remember to #import "Person.h" in the implementation file, although using xcode to choose the subclass should make that happen automatically.

###and then the main.m must import all the header/ interface files. It must import the parent class Shape.h or Person.h and then all the kids too... Circle.h and Square.h and Employee.h as the case may be.

###The isa pointer stands for "is a." it is the only instance variable of NSObject. All classes inherit, directly or indirectly, from NSObject. 

### if a message is sent to a class, trying to use a method, the isa pointers point back to parent classes where this method may reside.

###
