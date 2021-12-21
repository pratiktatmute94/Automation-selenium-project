# Automation-selenium-project
# This is my selenium project...
package control;

public class Elseif {
	
	public static void test1()
	{
		int noofdays = 32;
		if (noofdays==31) 
				{
			System.out.println("jan,march,may,july,aug,oct,dec");
				}
		else if(noofdays==30)
		{
			System.out.println("apr,june,sept,nove");
		}
		else if(noofdays==28 || noofdays ==29)
		{
			System.out.println("feb");	
		}
		else 
		{
			System.out.println("invalid month");
		}
	}
	public static void main(String[] args) {
		test1();	
	}	 
	}



