## OOP
- Class is the container for similar type methods and interfaces, it represents a general form of something like a general rectangle, while object is an instance of the class that have its own states and behaviors, example: a rectangle with specific width and height.   
- Inheritance: it is a useful concept in OOP, it provides code reusability and satisfy DRY (Don't Repeat Your Self) principle. It allows similar type classes to inherits states, behaviors and interfaces from other classes. There is a class called super class, example: Student, and a sub-class that inerits from super classes common states and behaviors, example: FirstYearStudent. 

## Java *Static* keyword
*Static methods* are also called *class methods*, because the are bind to the class itself not to the object and can be used directly by the class name without need to inistaniate an object. Making a variable *Static* means we can access it without need to inistaniate an object from the class, `ClassName.variableName`.

- *Design Pattern*: is a set of best practices that can help you in your code to solve problems and make your code efficient, and easy to track and edit without any problems. Example: *Strategy pattern:* it is used to separate the classes (parts) from your code that are continuously changing from the parts that remains the same.
- *Singelton:* it is a design pattern that ensures that a class can only have one object.
To create a singleton class, a class must implement the following properties:
- Create a private constructor of the class to restrict object creation outside of the class.
- Create a private attribute of the class type that refers to the single object.
- Create a public static method that allows us to create and access the object we created. Inside the method, we will create a condition that restricts us from creating more than one object.
