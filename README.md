# Assingment_BTech2026_-2201920100198-cse-D
oops problem and solution (c++)

problem 1: (03-02-2025): Area of Rectangle

Problem statement
Design a class called Rectangle. It contains two data members as length(L) and breadth(B); and a member function getArea(). The member function computes the area of the given rectangle and returns it to the caller.

Note:

Area of a rectangle = length x breadth
Data Members:
1. length: Length of the rectangle
2. breadth: Breadth of the rectangle 
Member Functions:
1. getArea(): that calculates the area of the rectangle and returns the value.
Note:

You do not have to take input, just create the Class and set the name of the Data Members and function as given in the above discription.
Detailed explanation ( Input/output format, Notes, Images )
Constraints:
0 <= L, B <= 100
Sample Input 1:
4 20
Sample Output 1:
80
Explanation of Sample Input 1:
Length of the rectangle is 4 and breadth is 20. 
Hence the area of the rectangle is (length*breadth). 
So the answer is 4*20=80.
Sample Input 2:
2 10
Sample Output 2:
20
Explanation of Sample Input 2:
Length of the rectangle is 2 and breadth is 10. 
Hence the area of the rectangle is (length*breadth). 
So the answer is 2*10=20.



problem 2:(04-02-2025)  (Print Name and age)

Problem statement
Create a class named Person with a string variable 'name' and an integer variable 'age,' such that these variables are not accessible outside the class and implement a way to initialize the variables and print the variables.

Functions: 1.setValue- that sets the variables value. 2.getValue- that prints the variables value.
Detailed explanation ( Input/output format, Notes, Images )
Sample Input 1:
Afzal
67
Sample Output 1:
The name of the person is Afzal and the age is 67.
Sample Input 2:
Ali
30
Sample Output 2:
The name of the person is Ali and the age is 30.
Explanation of Sample Input 1:
The input name is Ali and the input age is 30 which is printed in the specified format.

problem 3:(05-02-2025)  (Car Class)

Problem statement
Design a class Car having parameterized constructor that takes two arguments as an input i.e noOfGear and color and a printCarInfo method that prints the CarInfo i.e noOfGear and color.

Design another class RaceCar having parameterized constructor has an additional attribute maxSpeed and printRaceCarInfo method that prints the RaceCarInfo i.e noOfGear, color and maxSpeed.

Note: You have to create an object of class RaceCar and call the printRaceCarInfo method.

Detailed explanation ( Input/output format, Notes, Images )
Sample Input 1:
5
red
1000
Sample Output 1:
noOfGear: 5
color: red
maxSpeed: 1000
Explanation of Sample output 1:
When we call the printInfo function, all the info related to the car will be printed the same as the above format.

problem 3:(06-02-2025)  (Multilevel Inheritance)

Problem statement
Create a class GrandFather that has a parameterized constructor and a grandFatherName attribute.

Create another class Father that inherits the property of GrandFather and has a parameterized constructor with an additional argument fatherName.

Create another class Son that inherits Father's property and has a parameterized constructor with an additional argument sonName and a printName method that prints the sonName,fatherName, and grandFatherName into the format as shown below in SampleOutput 1.

You need to create the object of Son class and pass the value of sonName,fatherName,grandFatherName as 'Saurabh', 'Ramesh', and 'Suresh' respectively and call the printName method.

Sample Output 1 :
sonname:  Saurabh
fathername:  Ramesh
grandfather:  Suresh
Note:
Keep all the attribute value static as  above mention in sample output 1.


problem 4:(07-02-2025)  (Shape and Overriding)

Problem statement
Create a Class Shape having a field shapeType and a function printMyType.

Create another class, Square and Rectangle, which inherits the Shape class and has additional fields length and breadth. Both Square and Rectangle classes will have two functions calculateArea, which will return the object's area, and printMyType, which will print the type of the object.

Inside the main, first create the object of class Square and have a length equal to 5 and call the printMyType then calculateArea method after creating the object of class Rectangle having the length equal to 5 and breadth equal to 4 and again call the printMyType and calculateArea method.

Sample Output 1 :
square
25
rectangle
20
Explanation of Sample output 1:
Firstly we are creating the object of class Square with mentioned length 5 and calling the functions printMyType which output square and then calculateArea which returns 25 and hence printed. Similarly, it is done for the Rectangle class.


problem 5:(08-02-2025)  (Complex Number Class)

Problem statement
A ComplexNumber class contains two data members: one is the real part (R) and the other is imaginary (I) (both integers).

Implement the Complex numbers class that contains the following functions -

1. constructor
You need to create the appropriate constructor.

2. plus -
This function adds two given complex numbers and updates the first complex number.

e.g.

if C1 = 4 + i5 and C2 = 3 +i1
C1.plus(C2) results in: 
C1 = 7 + i6 and C2 = 3 + i1
3. multiply -
This function multiplies two given complex numbers and updates the first complex number.

e.g.

if C1 = 4 + i5 and C2 = 1 + i2
C1.multiply(C2) results in: 
C1 = -6 + i13 and C2 = 1 + i2
4. print -
This function prints the given complex number in the following format :

a + ib
Note: There is space before and after '+' (plus sign) and no space between 'i' (iota symbol) and b.

Detailed explanation ( Input/output format, Notes, Images )
Sample Input 1 :
4 5
6 7
1
Sample Output 1 :
10 + i12
Sample Input 2 :
4 5
6 7
2
Sample Output 2 :
-11 + i58


problem 6:(09-02-2025)  (Classes   hackerrank):(https://www.hackerrank.com/challenges/c-tutorial-class/problem?isFullScreen=true)

Classes in C++ are user defined types declared with keyword class that has data and functions . Although classes and structures have the same type of functionality, there are some basic differences. The data members of a class are private by default and the members of a structure are public by default. Along with storing multiple data in a common block, it also assigns some functions (known as methods) to manipulate/access them. It serves as the building block of Object Oriented Programming.

It also has access specifiers, which restrict the access of member elements. The primarily used ones are the following:

public: Public members (variables, methods) can be accessed from anywhere the code is visible.
private: Private members can be accessed only by other member functions, and it can not be accessed outside of class.
Class can be represented in the form of

class ClassName {
    access_specifier1:
        type1 val1;
        type2 val2;
        ret_type1 method1(type_arg1 arg1, type_arg2 arg2,...)
        ...
    access_specifier2:
        type3 val3;
        type4 val4;
        ret_type2 method2(type_arg3 arg3, type_arg4 arg4,...)
        ...
};
It's a common practice to make all variables private, and set/get them using public methods. For example:

class SampleClass {
    private:
        int val;
    public:
        void set(int a) {
            val = a;
        }
        int get() {
            return val;
        }
};
We can store details related to a student in a class consisting of his age (int), first_name (string), last_name (string) and standard (int).

You have to create a class, named Student, representing the student's details, as mentioned above, and store the data of a student. Create setter and getter functions for each element; that is, the class should at least have following functions:

get_age, set_age
get_first_name, set_first_name
get_last_name, set_last_name
get_standard, set_standard
Also, you have to create another method to_string() which returns the string consisting of the above elements, separated by a comma(,). You can refer to stringstream for this.

Input Format

Input will consist of four lines.
The first line will contain an integer, representing the age. The second line will contain a string, consisting of lower-case Latin characters ('a'-'z'), representing the first_name of a student.
The third line will contain another string, consisting of lower-case Latin characters ('a'-'z'), representing the last_name of a student.
The fourth line will contain an integer, representing the standard of student.

Note: The number of characters in first_name and last_name will not exceed 50.

Output Format

The code provided by HackerRank will use your class members to set and then get the elements of the Student class.

Sample Input

15
john
carmack
10
Sample Output

15
carmack, john
10

15,john,carmack,10
