 JAVA TUTORIAL
================
****************


To create a java program you need to use a text editor ( e.g notepad or notepad++) or a or an Integrated Developement Environment (e.g Eclipse, netbeans).

In java everything is a class or an object and therefore all the  functions, methods, objects, attributes, variables, storage areas, for example, that your program is going to require should be defined in a class.

These classes usually start with key words that determine the scope of the class. For the classes that are to be used by all the classes the program,  we use keyword public as we see in the examples below:

Example 1:
***********

	public class classname
		{
			public static void main(String[] args)
				{
					System.out.println("text");
				}
		}

	(When executed the above class will print out "text")

Now to break it down in order of appearance:
********************************************
public - when used tells the compiler that the class can be used by 			every other class
class - Keyword to indicate that we are creating a class
static - Indicates that only the class that it is being created from 		can call it. 
void - Indicates that the class doesn't return anything after it has 	finished executing.
main - This is a function that is required in every java program and is 	the one that is executed first. It can have arguments or not, 	in this case it does an array of strings.
system.out - An object that prints out (to the screen) in different 	ways.

println - outputs data in a line

That is a simple and basic class, now to create a class variable we will build upon the example above and as the name suggests we add variables to the class.


Variables
*********
These are storage areas and are case sensitive. When creating them you have to specify which data type you are expecting to accomodate in the array, using String (with a capital S) means the variable will hold only string characters so forth.

Example 2
**********

	public class classname
		{
			static String randomString = "String";
	
			static final double PI = 3.14;	

			public static void main(String[] args)
				{
										System.out.println(randomString);
				}
		}

(When executed the above class will print out "String")

Final - Used if you want a variable to be constant throughout the 		program.It is common practice that the variable name is usually 	in uppercase.

Before using a variable you must declare it using the data type and you can assign the value or declaration statement at declaration or elsewhere in the class.

Example 3
*********
	public class classname
		{
			static String randomString = "String";
	
			static final double PI = 3.14;	

			public static void main(String[] args)

				{
					int number1 = 23 // assignment at declaration
					int number2 = number1 + 1 // declaration statement
					System.out.println(number2);

				}
		}

When executed the above class will print out 24

worth noting
------------
We have seen int, String and double data types, other primitive types in java and the only thing that makes them different is the values they can hold,   
byte - (biggest 127) (smallest -127)
short - (biggest 32767 smallest -32768)
int - (biggest around 2.1 trillion)
long - (biggest 9220000000000000000L) ends with an L
float - decimal point ends with F(approx 6 decimal places)
double - a bigger and more precise float (app 15 decimal places)
boolean - Either true or false (lowercase)
char - either number representing ASCII character codes or string if 		surrounded by quotes. It can contain escaped characters '\f'.
String - characters inside double quotes "12anyth" and you can 		translate any type to string using -type.toString- method. to 		translate a string into an int you use		-Integer.parseInintString)
int - whole number

casting
*******
This is translating one primitive type to another primitive type
and we use (double), (int), (float), (byte), (long), (short). 

example
*******

int intNo = (int) aDoubleValue;


  




