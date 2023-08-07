## Packages
Packages in java are containers that collect a related types of: classes, interfaces, methods, variables. they are used to make a efficient code structure.There are two types of packages in java:
1. **Built-in** packages: they exists in the JDK, you only need to import them in your code and access their features. example: 
java.util, java.lang, java.awt,java.sql
2. **User-defined**  packages: they are created by the user.
*How to create User-defined package in  IntelliJ:*
1. click on the source(src) and choose new package.
2. Enter the package name beside the keyword package , then the file will be created, and you can add classes and interfaces inside it.
3. Import it in your code by using `import PackageName` or import specific class `import PackageName.className`.

## Loops
1. **For** loop: it repeats a certain operations on the code by using a counter and a condition on it.
2. **While** loop: it repeates a certain operations on the code by checking a boolean-expression, in case the expression returned **true** the operations inside the loop will be executed. We can create infinite loop uisng While loop.
3. **Do-while** loop: the only difference between it and the While loop that the operations inside it will be executed at least once even the expression returns **false**. Because the it execute the operations then check the expression.

## Arrays
- Three buit-in methods for arrays: `Arrays.toString()`, `Arrays.sort()`, `Arrays.binarySearch()`.
- The size of arrays are determined: dataType arrayName[]= new dataType[arraySize:number or varaiable], example: `int a[] = new int[5]`.