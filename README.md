# livesessionscode
package com.qa.cardemo;
import static org.junit.jupiter.api.Assertions.assertEquals;
import org.junit.jupiter.api.AfterEach;
import org.junit.jupiter.api.BeforeEach;
import org.junit.jupiter.api.Test;
public class TestCar {
	Car car;
	
	@BeforeEach
	public void setUp() {
		car = new Car("Ford");
	}
	
	@AfterEach
	public void tearDown() {
		car = null;
	}
	
	@Test
	void testCarAccelerate() {
		System.out.println("@test");
		car.accelerate(10);
		assertEquals(50, car.getSpeed());
	}
}





 <dependencies>
  <!-- https://mvnrepository.com/artifact/org.seleniumhq.selenium/selenium-java -->
<dependency>
    <groupId>org.seleniumhq.selenium</groupId>
    <artifactId>selenium-java</artifactId>
    <version>4.18.1</version>
</dependency>
  <!-- https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api -->
<dependency>
    <groupId>org.junit.jupiter</groupId>
    <artifactId>junit-jupiter-api</artifactId>
    <version>5.10.2</version>
    <scope>test</scope>
</dependency>
  		<!-- https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-engine -->
		<dependency>
			<groupId>org.junit.jupiter</groupId>
			<artifactId>junit-jupiter-engine</artifactId>
			<version>5.10.0</version>
			<scope>test</scope>
		</dependency>
    <dependency>
      <groupId>junit</groupId>
      <artifactId>junit</artifactId>
      <version>3.8.1</version>
      <scope>test</scope>
    </dependency>
  </dependencies>
