**************************
==========================
JAVA - Derek Banas video 4
==========================
**************************


******************
Loop - While loops
******************

---------
Example 1
---------

public class name4 {

	public static void main(string[] args)
	{
		int i = 1;
		while(i <= 20) 
		{
			System.out.println(i);
			i++;
		}
	}
}

	OUTPUT: print out numbers 1 to 20

You can nest it with an if or for statements to provide spice

---------
Example 2
---------

public class name4 {

	public static void main(string[] args)
	{
		int i = 1;

		while(i <= 20) 
		{
			if(i == 3)
			{
				i+=2;
				continue;
			}
			System.out.println(i);
			i++;
		}
	}
}

	OUTPUT: print out numbers 1 to 20 but will skip 3 & 4

Using a break statement
---------
Example 3
---------

public class name4 {

	public static void main(string[] args)
	{
		int i = 1;
		while(i <= 20) 
		{
			if(i == 3)
			{				
				i+=2;
				continue;
			}
			if (i > 10)
			{
				break;
			}

			System.out.println(i);
			i++;
		}
	}
}

	OUTPUT: print out numbers 1 to 9 and will skip 3 & 4

Something cool : calculating pi
---------
Example 4
---------

public class name4 {

	public static void main(string[] args)
	{

		double myPi = 4.0;
		double j = 3.0;

		while(j <= 10001) 
		{

			myPi = myPi - (4/j) + (4/(j+2));
			j +=4
			System.out.println(myPi);
		
		}
		
		System.out.println("Value of PI " + Math.PI);
	}
}

	NOTE: The more the loops the closer the value gets

loop until user says stop
---------
Example 5
---------
public class name4 {

	static Scanner userInput = new Scanner(System.in);

	public static void main(string[] args)
	{

		String contYorN = "Y";
		int h = 1;

		while(contYorN.equalIgnoreCase("y")) 
		{

			system.out.println(h);
			system.out.print("Continue y or n? ");
			contYorN = userInout.nextLine();//accept string from user
			h++;		
		}		
	}
}

	OUTPUT: will print 1 then print 'Continue y or n?' if user puts y 			or Y then it will print the next number, else an n or any 			other letter it will break the loop


worth noting
------------
- the counter or loop iterator is created outside the loop statement
- continue tells the loop to jump out of the nested loop and continue with the execution.
- if we want to print only even numbers we can use if((i%2) == 0);
- Break will exit and stop the loop if the code of block is true.


*****************
Loop - Do - while
*****************

A while do while loop is used when you want the code to run atleast once

---------
Example 6
---------

public class name4 {
	public static void main(string[] args)
	{
		int k = 100;

		do 
		{
			system.out.println(k);
			k++;
			
		} while (k < 10);		
	}
}

	OUTPUT: prints out 100 before breaking


****************
Loops - for loop
****************

public class name4 {
	public static void main(string[] args)
	{
		for(int i=10; i>=1; i--) 
		{
			system.out.println(i);
			
		}		
	}
}

	OUTPUT: prints out numbers from 10 to 1

worth noting
------------
if you do a system.out.println outside of the loop as is it will throw an erro because var i was declared inside the for loop, however you can declare the variables outside and this allows for accessability outside the for loop.