
This is a Java-based Shape Calculator that computes area, perimeter, and volume for various shapes using OOP principles. 
It implements abstract classes and interfaces for a structured and modular approach.


Features -

Supports Circle, Rectangle, Square, Sphere, Cylinder, and Equilateral Pyramid.

Uses an abstract class (Shape) for common properties and methods.

Implements a Volume interface for 3D shapes.

Menu-driven program for user-friendly interaction.

Organized into multiple Java files for better modularity.


Methods and Functions - 

1️. Abstract Class - Shape

The Shape class provides a base structure for all shapes.

Methods:

Shape(String shapeName) → Constructor to initialize the shape.

calculateArea() → Abstract method for area calculation (Implemented in subclasses).

calculatePerimeter() → Abstract method for perimeter calculation (Implemented in subclasses).

2️. Interface - Volume

The Volume interface is used for 3D shapes that have volume.

Methods:

calculateVolume() → Abstract method (Implemented in Sphere, Cylinder, and Pyramid).

3️. Concrete Shape Classes

🔹 Circle (Circle.java)

Extends Shape and implements area & perimeter calculations.

Methods:

Circle(double radius) → Constructor to initialize the circle.

calculateArea() → Returns π * radius².

calculatePerimeter() → Returns 2 * π * radius.

🔹 Rectangle (Rectangle.java)

Extends Shape and implements area & perimeter calculations.

Methods:

Rectangle(double length, double width) → Constructor to initialize the rectangle.

calculateArea() → Returns length * width.

calculatePerimeter() → Returns 2 * (length + width).

🔹 Square (Square.java)

Extends Rectangle (inherits its properties).

Methods:

Square(double side) → Constructor to initialize the square.

calculateArea() → Returns side².

calculatePerimeter() → Returns 4 * side.

🔹 Sphere (Sphere.java)

Extends Shape and implements Volume for volume calculation.

Methods:

Sphere(double radius) → Constructor to initialize the sphere.

calculateArea() → Returns 4 * π * radius².

calculatePerimeter() → Not applicable for a sphere.

calculateVolume() → Returns (4/3) * π * radius³.

🔹 Cylinder (Cylinder.java)

Extends Shape and implements Volume for volume calculation.

Methods:

Cylinder(double radius, double height) → Constructor to initialize the cylinder.

calculateArea() → Returns 2 * π * radius * (radius + height).

calculatePerimeter() → Returns 2 * π * radius.

calculateVolume() → Returns π * radius² * height.

🔹 Equilateral Pyramid (Pyramid.java)

Extends Shape and implements Volume for volume calculation.

Methods:

Pyramid(double base, double height) → Constructor to initialize the pyramid.

calculateArea() → Returns Base Area + 4 * (Triangle Side Area).

calculatePerimeter() → Returns 4 * base length.

calculateVolume() → Returns (1/3) * Base Area * Height.

4️. Main Class (Main.java)

The menu-driven program that interacts with users and performs operations based on user input.

Methods:
displayMenu() → Displays available shape options.

getShapeInput() → Takes user input for shape selection.

processShape() → Calls the respective shape’s methods and displays results.
