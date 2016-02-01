**************************
==========================
JAVA - Derek Banas video 3
==========================
**************************

********************
Arithmetic operators
********************

+ : Addition
- : Subtraction
* : Multiplication
/ : Division
% : Modulus
++: Increament
--: Decreament


********************
Relational OPerators
********************

Java has 6 operational operators and they are:

> : Greater than
< : Less than
== : Equal to
!= : Not equal to
>= : Greater than or equal to
<= : Less than or equal to

---------
Example 1
---------

public class name3 {

	public static void main(String[] args)
	{

		int randomNumber = (int) (Math.random() * 50);

		if (randomNumber < 25) 
		{

			System.out.println("The random Number is Less than 25");

		}
		
		System.out.println("The random number is " + randomNumber);

	}

}

	OUTPUT: If the random number is less than 25 then it will print out 			'The numer is less than 25' then print out the number if not 		it will just print out the random number.
*****************
Logical Operators
*****************

Java has 6 logical operators

! : Converts boolean value to its opposite form 
&& : Returns true if both the boolean value on the left and the value on the right are true
| : Returns true if any or both of the boolean values on the right or left is true
||: Returns true if any or both of the boolean values on the right or left is true
^ : Returns true if there is one true and one false value in the equation.

********************************
conditional (terniary) statements
********************************

Assigns one value or another based on a certain condition.
? :

---------
Example 2
---------

public class name3 {

	public class void main(String[] args)
	{

		int valueOne = 1;
		int valueTwo = 2;

		int biggestValue = (valueOne > ValueTwo) ? valueOne : valueTwo;	
	
		System.out.println(biggestValue);

	}

}

	OUTPUT: If valueOne is bigger then it will assign it to biggerValue 		and print it out else valueTwo.


***************************
Loop: If - else and else if
***************************

This is a loop statement.

if - in a class will execute the if block(the block inside the if statement) only when the if expression is true.
else if - is used when writing multiple if statements.
else - executes only when the if statement is false and should be there to catch exceptions to avoid crashing of the program.

---------
Example 3
---------

public class name3 {

	public static void main(String[] args)
	{

		int randomNumber = (int) (Math.random() * 50);

		if (randomNumber < 25) 
		{

			System.out.println("The random Number is Less than 25");

		} else if (randomNumber => 90) 
		{

			System.out.println("The random Number is greater than 90");

		} else {

			System.out.println("Nothing worked");

		}

		System.out.println("The random number is " + randomNumber);


	}

}

	OUTPUT: If the random number is less than 25 then it will print out 			'The number is less than 25' and if the number is greater 			than 90 it will print the if block with  that expression 	 		print out the number if not it will just print out the 				random number. 

worth noting 
------------
- Whenever there are multiple if statements (else if) when the first if statement returns true noe of the other if statements will be checked.
- Using a ! before the parenthesis checks for the value that is not the expression.

---------
Example 5
---------

public class name3 {

	public static void main(String[] args)
	{

		int randomNumber = (int) (Math.random() * 50);

		if !(randomNumber < 25) 
		{

			System.out.println("The random Number is Less than 25");

		}  

		System.out.println("The random number is " + randomNumber);


	}

}

	OUTPUT: If the random number is not less than 25 then it will print 			out 'The numer is less than 25' then print out the number if 		it is will just print out the random number. 

  

******************
Loops: Switch case
******************

This is a loop statement that is used when there are a limited number of possible values.

---------
Example 4
---------

public class number3 {

	public static void main(string[] args) 
	{

		char theGrade = 'B';

		swirch (theGrade)
		{
		case 'A':
			System.out.println("Great job");
			break;
		case 'B':
			System.out.println("Good Job");
			break;
		default:
			System,out.println("You fialed");
			break;

		}

	}
}

	OUTPUT: print out 'Good job'

worth noting
------------

- we use break when we want the loop to stop if the case statement is true.
- The default where it defaults to in case none of the case statements is true.
- Switch case is case sensitive and to catch the exceptions where statement exaluates true in both lower and upper case you will have to specify example

case 'a':
case 'A':
	system..... 