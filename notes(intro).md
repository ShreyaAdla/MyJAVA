JAVA INTRODUCTION
JDK - JAVA DEVELOPMENT KIT - it contains developer tools that help us code
      JRE: JAVA RUNTIME ENV - it contains libraries and tool kits.
          JVM : JAVA VIRTUAL MACHINE -  which translates byte code to machine code 

SOURCE CODE IN JAVA:
**package first;
public class Main {
	public static void main(String[] args) {
		// TODO Auto-generated method stub
	}
}**
Class main is "main"
Program cannot run without main method i.e, public static void main....
**System.out.print("write anything to display");** ------- to print output
**println or \n** for next line but do not use both. If you use both a new empty line will be created.
**\t**   will add space 
**sysout + ctrl + space** for System.out.println
**VARIABLES**
**DATATYPES**
1.. Boolean - 1 bit --true or false
2.. int   - 1 byte --  -2 to 2
3.. double   - 8 bytes -- 3.1415(upto 15 digits)
4.. char - 2 bytes -- single character/letter/ASCII value - single quotes -- 'f'
5.. string (reference datatype) - varies -- "Hello World"
6..float - 4 bytes -- 3.14(upto 6-7digits)
7..long - 8 bytes -- (used to store long number like speed of lioght as int cannot store large value)
8..byte - 1 byte --
9..short - 2 bytes
char is primitive && string is reference
primitive -- 8 types , stores data , holds 1 value, less memory, faster
refernece -- unlimited(user defined) , stores address , hold more than 1 value, more memory, slower
**CREATING VARIABLE**
datatype+vale
int x;           DECLARATION
x = 123;         ASSIGNMENT
int x = 123;     INITIALIZATION

		//int x;  //declaration
		//x=123;  //assignment
		int x = 123; //initialization
		double y = 3.14;
		boolean z= true;
		char symbol = '@';
		String name = "Shreya";
		//String S should be capital as it is reference data type
		System.out.println("My number is : "+x);
		System.out.println("Number :"+y );
		System.out.println(z);
		System.out.println(symbol);
		System.out.println(name);
		System.out.println("My name"+ " " +  " " + symbol   + " " + name);

 **OUTPUT** = My number is : 123
		   Number :3.14
		   true
	           @
                   Shreya
                   My name  @ Shreya

**SWAPPING VARIABLES**
		String a = "water";
		String b = "juice"; 
		//b = a;
		//Creating another variable
		String temp ;
		temp = a;   //temp = a(water)
		a=b;        //a = juice 
		b= temp;    // b = water
		System.out.println("a: " + a);
		System.out.println("b: " + b);
   **OUTPUT** : a: juice
                b: water

**USER INPUT** IN JAVA
WE need to use **Scanner** class. So we need to import the class **import java.util.Scanner;**
 Procedure: first create scanner object i.e, Scanner scanner = new Scanner(System.in);
            next ask question
	    next ask user to give i/p (scanner.nextLine(), scanner.nextInt())
            next write the answer
**Program for USER INPUT**
     	        //USER INPUT 
		//USE Scanner for user input
		// first create Scanner object as below
		Scanner scanner = new Scanner(System.in);
		
		// Asking question
		System.out.println("What is your name?");
		//using scanner 
		String myname = scanner.nextLine();
		
		//Asking 2nd question
		System.out.println("What is your age?");
		//using scanner for 2nd
		int myage = scanner.nextInt();
		scanner.nextLine();    // THIS IS IMPT TO ADD TO CLEAR THE SCANNER 
		//Asking 3rd Question
		System.out.println("What is your fav food?");
		//using scanner for 3rd
		String myfood = scanner.nextLine();
		
		
		//printing answer
		System.out.println("My name is : " + myname);
		System.out.println("My age is : " + myage);
		System.out.println("My fave food is : " + myfood);

Output:   What is your name?
	 Shreyau
	 What is your age?
	 24
	 What is your fav food?
	 Biryani
	 My name is : Shreyau
	 My age is : 24
	 My fave food is : Biryani

**EXPRESSIONS**
	Expression = operators + operands
 	operators = +,_,/,% (% gives remainder)
	operands = values,variables,numbers, quantity
 	//EXPERSSIONS
		double num = 10;
		//num = num + 10;
		//num = num - 10;
		//num = (double)num / 3; //(Divident as answer)(to get decimal use "DOUBLE")
		
		//num = num % 3;   // (remainder as answer)
		//num++; //+1
		//num--; //-1
		
		System.out.println(num);
  **Creating a basic GUI (GRAPHICAL USER INTERFACE) Program**
  		
    		String name = JOptionPane.showInputDialog("What is ur name?");
		JOptionPane.showMessageDialog(null, "Hello " + name);
		//when u r using "showInputDialog" it is going to return string. So we need to convert it to integer
		**TO CONVERT STRING INTO ANY OTHER DATATYPE USE the-- interger: use Integer.parseInt()**
		
		int age = Integer.parseInt(JOptionPane.showInputDialog("what is ur age?"));
		JOptionPane.showMessageDialog(null, "Your age is " + age);
		
		double height = Double.parseDouble(JOptionPane.showInputDialog("what is ur height?"));
		JOptionPane.showMessageDialog(null, "Your height is " + height + " in cm.");
  **MATHEMATICS IN JAVA**
  		// MATHEMATICAL FUNCTION
		/*
		double x = -3.14;
		double y = 4;
		double z;
		//z= Math.max(x, y);  //Finding max number
		z= Math.min(x, y); //Finding minimum number
		//z= Math.abs(x);  // if the given number is negative it makes positive
		System.out.println(z);
		*/
		// FINDING A HYPOTENUSE OF TRIANGLE BY ASKING USER THE VALUES
		Scanner scanner = new Scanner(System.in);
		System.out.println("Enter x: ");
		double x = scanner.nextDouble();
		System.out.println("Enter y: ");
		double y = scanner.nextDouble();
		double z= Math.sqrt(x*x + y*y);
		System.out.println("the hypotenuse is : " + z);
  **OUTPUT** :  Enter x: 
		4
		Enter y: 
		5
		the hypotenuse is : 6.4031242374328485
  

         
		

 

