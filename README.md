# Opencart

package org.javaselenium;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.annotations.Test;

public class Demo {
	
	@Test
	
	private void tablehandle()  {
		
		WebDriver driver = new ChromeDriver();
		
		driver.get("https://demowebshop.tricentis.com/");
		
		driver.findElement(By.className("ico-login")).click();
		driver.findElement(By.id("Email")).sendKeys("suryatick2000@gmail.com");
	    driver.findElement(By.id("Password")).sendKeys("96takeoff");
        driver.findElement(By.xpath("//input[@class='button-1 login-button']")).click();
	    driver.findElement(By.linkText("Computers")).click();
	   driver.findElement(By.linkText("Desktops")).click();
	   driver.findElement(By.linkText("Build your own computer")).click();
	   driver.findElement(By.id("product_attribute_16_5_4")).click();
	   driver.findElement(By.linkText("2.2 GHz Intel Pentium Dual-Core E2200")).click();

}

}
