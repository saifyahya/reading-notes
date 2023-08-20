## OOP
- Class is the container for simillar type methods and interfaces, it represents a general form of something like a general rectangle, while object is an instance of the class that have its own states and behaviours, example: a rectangle with specific width and height.   
- Inheritance: it is a useful concept in OOP, it provides code reusability and satisfy DRY (Don't Repeat Your Self) prinsiplie. It allows simillar type classes to inherit states, behaviours and interfaces from other classes. There is a class called super class, example: Student, and a sub-class that inerits from supder classes common states and behaviours, example: FirstYearStudent. 

## Java *Static* keyword
*Static methods* are also called *class methods*, because the are bind to the class itself not to the object, and can be used directly by the class name without need to inistantiate an object. Making a variable *Static* means we can access it withou nedd to inistantiate a n object from the class, `ClassName.variableName`.

- *Design Pattern*: is a set of best practises that can help you in your code to solve problems and make your code efficient, and easy to track and edit without any problems. Example: *Strategy pattern:* it is used to seperate the classes (parts) from your code that are continueosly changing from the parts that remains the same.
- *Singelton:* it is a design pattern that ensures that a class can only have one object.
To create a singleton class, a class must implement the following properties:
- Create a private constructor of the class to restrict object creation outside of the class.
- Create a private attribute of the class type that refers to the single object.
- Create a public static method that allows us to create and access the object we created. Inside the method, we will create a condition that restricts us from creating more than one object.