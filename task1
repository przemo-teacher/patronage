
package nowyprojekt;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.Assert;

public class myfirsttest {
WebDriver driver;

public void launchBrowser() {
	
	System.setProperty("webdriver.chromedriver", "/Users/user/Downloads/jars and drivers/chromedriver");
	driver= new ChromeDriver();
	driver.get("https://www.phptravels.net/login");
	WebElement username=driver.findElement(By.name("email"));
	WebElement password=driver.findElement(By.name("password"));
	WebElement login=driver.findElement(By.name("Login"));
	username.sendKeys("user@phptravels.com");
	password.sendKeys("demouser");
	login.click();
	String actualUrl="https://www.phptravels.net/account/dashboard";
	String expectedUrl= driver.getCurrentUrl();
	Assert.assertEquals(actualUrl, expectedUrl);
}
	public static void main(String[] args) {
	}
	
}
