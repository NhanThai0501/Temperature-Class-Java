# Temperature-Class-Java

Assignment Objects:

Look at and implement exercise # 8 from the book   

HOWEVER,   I find it a bit limiting.   

We can keep the Constructor that has a double as the parameter that specifies a temperature in Fahrenheit.  

Do do all the methods that they show.   

 

ADD 

Add a method to set the temperature given it is in Kelvin   

void setKelvin ( double tempInKelvin)

Add a method to set the temperature given it is in Celsius:

void setCelcius ( double tempInCelsius ) 

 

Please document your test cases:

That means you should log each value/function that you use and the result.   

 

 

 

 

DISCUSSION QUESTIONS:

How many data items are private and hidden inside the class?
Do you have 1, 2 or 3 data items in the class?   
Why did you implement that way ?
How many test cases are need and why?
 Did you exercise all the lines of code in the class?
 

Question # 8 from the book:

 

Write a Temperature class that will hold a temperature in Fahrenheit,   And provide methods to get the temperature in Fahrenheit, Celsius, and Kelvin.   The class should have the following field

fahrenheit - A double that holds a Fahrenheit Temperature.

The class should have the following methods:

Constructor - The constructor accepts a Fahrenheit temperature ( as a double) and stores it in the ftemp field. 
setFahrenheit - The setFahrenheit method accepts  a Fahrenheit temperature ( as a double) and stores it in the ftemp field. 

getFahrenheit - Returns the value of the ftemp field, as a Fahrenheit temperature.
celsius - Returns the temperature in Celsius.
kelvin - Returns the value of the ftemp field converted to Kelvin.  
Use the following formula to convert the Fahrenheit temperature to Celsius

     Celsius = ( 5/9 ) * ( Fahrenheit - 32.0 )

Use the following to convert Fahrenheit to Kelvin:

Kelvin = ( ( 5/9 ) * ( Fahrenheit - 32.0 )  + 273.15

8. Temperature class
Write a Temperature class that will hold a temperature in Fahrenheit, and provide methods to get the temperature in Fahrenheit, Celsius, and Kelvin. The class should have the	
following field:
•	 ftemp	–	A	double that holds a Fahrenheit temperature.
The class should have the following methods:
•	 Constructor	–	The	constructor	accepts	a	Fahrenheit	 temperature	 (as	a	double) and
stores it in the ftemp field.
•	 setFahrenheit – The setFahrenheit method accepts a Fahrenheit temperature (as a
double) and stores it in the ftemp field.
•	 getFahrenheit – Returns the value of the ftemp field, as a Fahrenheit temperature (no
conversion required).
•	 getCelsius – Returns the value of the ftemp	field	converted	to	Celsius.
•	 getKelvin – Returns the value of the ftemp field converted to Kelvin.

Use	the	following	formula	to	convert	the	Fahrenheit	temperature	to	Celsius:
Celsius = (5/9) * (Fahrenheit -	32)

Use the following formula to convert the Fahrenheit temperature to Kelvin:
Kelvin = ((5/9) * (Fahrenheit - 32) + 273)

Demonstrate the Temperature class by writing a separate program that asks the user for a
Fahrenheit temperature. The program should create an instance of the Temperature class,
with the value entered by the user passed to the constructor. The program should then call
the	object’s methods	to	display	the	temperature	in	Celsius	and	Kelvin.
