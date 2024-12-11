# Task05
1. palindrome
package scanner;
import java.util.Scanner;
public class Palindrome 
{
	public Palindrome()
	{
	}
	public static void main(String[] args)
	{
		Scanner scanner = new Scanner(System.in);
		 System.out.println("Enter a string:");
	        String input = scanner.nextLine();
	        String str = input.toLowerCase();

	        boolean isPalindrome = true;
	        int length = str.length();

for (int i = 0; i < length / 2; i++) {
	            if (str.charAt(i) != str.charAt(length - 1 - i)) {
	                isPalindrome = false;
	                break;
	            }
	        }
	        
	        if (isPalindrome) {
	            System.out.println("The string \"" + input + "\" is a palindrome.");
	        } else {
	            System.out.println("The string \"" + input + "\" is not a palindrome.");
	        }
	        scanner.close();
	    }
	
}

2.reverse string

package scanner;

import java.util.Scanner;

public class Reversedstring {

	public Reversedstring() 
	{
	}
	public static void main(String[] args) 
	
	{
Scanner scanner=  new Scanner(System.in);

System.out.println("Enter the String:");

String input = scanner.nextLine();

String Reversed="";

for (int i=input.length()-1; i>=0;i--);

System.out.println("Reversed String:" +Reversed);
scanner.close();

	}

}

3. pattern
   package scanner;
import java.util.Scanner;


public class pattern {

	public pattern() {
		
	}

	public static void main(String[] args) 
	{
		Scanner scanner = new Scanner(System.in);

     
        System.out.println("Enter the number of rows:");
        int rows = scanner.nextInt();

       
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print(j);
            }
            System.out.println(); 
        }

       
        scanner.close();
		

	}

}
4.Star pattern

package scanner;
import java.util.Scanner;

public class Starpttern {

	public Starpttern() {

	}

	public static void main(String[] args) {
	
		Scanner scanner = new Scanner(System.in);

	     
        System.out.println("Enter the number of rows:");
        int rows = scanner.nextInt();

       
        for (int i = 1; i <= rows; i++) {
            for (int j = 1; j <= i; j++) {
                System.out.print("*");
            }
            System.out.println(); 
        }

       
        scanner.close();
		
	}

}

5.Anna univ

package scanner;
import java.util.Scanner;
public class Ranking 
{
	public Ranking() 
	{
	}
	public static void main(String[] args) {
	
Scanner sc = new Scanner(System.in);

System.out.println("Enter the Student Mark:");

int mark = sc.nextInt();

if(mark < 0 || mark > 100)
{
	System.out.println("Invalid Entry, enter mark from 0 to 100:" +mark);
	
}
else
{
 String grade;
	if(mark==100)
	{
		grade ="S";
	}
	else if(mark >= 90)
	{
		grade ="A";
	}
	else if(mark >= 80)
	{
		grade ="B";
	}
	else if(mark >= 70)
	{
		grade = "C";
	}
	else if(mark >= 60)
	{
		grade = "D";
	}
	else if (mark >= 50)
	{
		grade ="E";
	}
	else if (mark<50)
	{
		grade ="F";
	}
	System.out.println("The grade is:" );
}
sc.close();
	}
}

6.hotel tarriff

package scanner;
import java.util.Scanner;

public class Hoteltariff {



	public Hoteltariff() {
		
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		
		String days;
		
System.out.print("Enter the number of days of stay:");
		int days1 = sc.nextInt();
		
System.out.println("Enter the number of month:");
			int month =sc.nextInt();
			
		
		
			boolean ispeakseason;
			switch(month) {
			case 1: //April;
			case 2: //May;
			case 3: //June;
			case 4: //November;
			case 5:// December;
				ispeakseason=true;
				break;
				default:
					ispeakseason=false;
				double totaltarriff;
				double roomrent = 0;
				if(ispeakseason)
					{
totaltarriff=roomrent*1.20 *days1;
					}
					else
					{
totaltarriff=roomrent*days1;	
					}
					

			}
System.out.println("The total tarriff is:" );
		

	        sc.close();
	}

}
