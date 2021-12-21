# Automation-selenium-project
# This is my selenium project...
package testNG;

import org.testng.annotations.AfterClass;
import org.testng.annotations.AfterMethod;
import org.testng.annotations.BeforeClass;
import org.testng.annotations.BeforeMethod;
import org.testng.annotations.Test;

public class Sample {
	 
	@Test(priority=1)        //  (priority=1) is for to run at first.
	public void TC01()       //  priority is not alphabet, not fraction only number...
	{
		System.out.println("Running TC01");
	}

	
	@Test(priority=3)        //  (priority=3) is for to run at 4th number..
	public void TC03()
	{
		System.out.println("Running TC03");
	}

	
	
	@Test(invocationCount=2)            // (invocationCount=4) is for 4 times run.
	public void TC02()
	{
		System.out.println("Running TC02");
	}
	
	
	@BeforeMethod
	public void loginToApplication()
	{
		System.out.println("login to app");
	}
	
	
	@AfterMethod
	public void logout()
	{
		System.out.println("log out to app");
	}
	

	@BeforeClass
	public void launchBrowser()
	{
		System.out.println("Browser launched");
	}
	
	
	@AfterClass(enabled = false)        // (enabled = false) is for not run.
	public void closeBrowser1()
	{
		System.out.println("Browser closed1");
	}
	
	

	@AfterClass     
	public void closeBrowser()
	{
		System.out.println("Browser closed");
	}
	
	
}

