# Code-Revision

The << operator put to writes it's 2nd argument onto the 1st. 
E.g. "Hello world" string literal is written onto the standard output stream std::cou t

\ + another character is a special character e.g. \n 

A double has 15 decimal points of precision and a float has 7, they are very similar.

Function overloading is calling a function the same name as another one. e.g. each print() prints it's arguments.

A type e.g. int (-235, 5), char ('a' 'z' '9') unsigned (non-negative integer), double. So a type defines a set of operations and a set of possible values (for an object). Floating point numbers are recognised by a decimal point or an exponent 3e-2. Integer literals - 0b is binary base 2 e.g. 0b10110111 0x - hexadecimal base 16 - 0 prefix indicates an octal base 8

An object is some memory which holds a value of some type.
A variable is a named object.

The key difference between Bitwise and Logical operators is that Bitwise operators work on bits and perform bit by bit operations while logical operators are used to make a decision based on multiple conditions.

x+=y // x = x+y
++x // increment
x∗=y // scaling: x = x*y
x/=y // scaling: x = x/y
x%=y // x = x%y

Scope and Lifetime
A declaration introduces it's name into a scope. Local scope, scope is from declaration to end of block (}) (local name). Class scope (member name) defined in a class outside of a function. Namespace member name if defined in a... namespace. A name not declared inside any other construct is called a global name and is said to be in the global namespace.

Objects without names e.c.t temporaries and objects created with new. An object created by new ‘‘lives’’ until destroyed by delete.

C++ immutability (unable to be changed).

An array of elements with type char can be declared as this char v[6];
A pointer can be declared like this char* p; //pointer to character. In declarations [] = 'array of' * = pointer to. A pointer variable can hold the address of an object of the appropriate type. char* p = &v[3] p points to v's 4th element.
* = contents of & = address of


Inheritance: When a class is based on another class and adds some more specific details. A line of inheritance usually goes from the most common and general aspect, all the way down to a point where it makes no more sense to be more specific. Example of this in the context of animals: Animal->Mamal->Rodent->Rat->RattusNorvegicus

Aggregates: Properties that "builds" the object. E.g. "This car is an aggregation of four wheels, a chassis, an engine, etc".

Attribute: Properties that describe the object, usually not part of its physical construction. E.g. Color, top speed, engine volume etc.

Encapsulation: The concept of concealing certain properties from the user, or to protect certain properties from being used incorrectly (and thereby damaging the object). E.g. You don't expose the gear-property of a car class to be altered freely. You encapsulate it and make sure Clutch() is called before SetGear().

Overriding: If a class inherits from another class, it also inherits methods from that class. Overriding is basically when the inheriting class replaces the implementation of such a method with its own required behaviour. Example of usage in next point.

Polymorphism: A difficult concept to grasp until you start using it practically. It means referring to a very specific kind of object, by using a generic reference which allows you to ignore the specific type (when you don't need to know it). E.g. If you want to "read" the license plate number property of every vehicle in a parking lot, you don't really care what the brand is, or even if it's a trailer or motorcycle or whatever. To be able to do this, we make sure the license plate number is a property in the most general class in the inheritance line (probably the Vehicle class). So you only have to deal with all the objects in a list by referring to them as their Vehicle class and then calling Vehicle::GetLicensePlateNumber(). Any vehicle requiring some special handling to retrieve the number can implement this behaviour by overriding the method and make it behave as required. So, a wide range of object types can be used as if they were of the same type, but can behave differently.
