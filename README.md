# Temperature-Class-Java
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package assign08temperatureclass;

import java.util.Scanner;

/**
 *
 * @author Nhan
 */
public class Assign08TemperatureClass {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Scanner keyboard = new Scanner (System.in);
        
        homeworkHeader();
        projectName();
        
//        menuDisplay();
//        choice ();
       
        
        double fahTemp, kelTemp, celTemp;
        
        System.out.print("Enter the Fahrenheit temperature: ");
        fahTemp = keyboard.nextDouble();

        Temperature fahrenheit = new Temperature(fahTemp);
        fahrenheit.setFahrenheit(fahTemp);
        
        
        System.out.println(fahrenheit.getFahrenheit());
        
        System.out.println("The temperature converted from Fahrenheit to Celsius is " + fahrenheit.getCelsius());
        System.out.println("The temperature converted from Fahrenheit to Kelvin is " + fahrenheit.getKelvin());
        
        
    }  
    
   
    static void homeworkHeader ()
    {
        System.out.println("Ticket : 86713");

        System.out.println( "Course : CMPR 112 ");

        System.out.println( "Student : Nhan Thai ");

        System.out.println( "Instructor : Joel Kirscher");

        System.out.println( "Environment: Win 10 NetBeans ");
    }
    
    static void projectName ()
    {
        String title = "Assign 8 Temperature Class\n";
        System.out.println("Project Name : " + title);
    }
    
    public static class Temperature
    {
        private double fahrenheitTemp;
        private double kelvinTemp;
        private double celsiusTemp;
        
        /**
         Constructor
         * @param ftemp 
         * @param tempInKelvin
         * @param tempInCelsius
         */
        public Temperature (double ftemp)  
        {
            fahrenheitTemp = ftemp;
        }
        
           
        public void setFahrenheit (double ftemp)
        {
            fahrenheitTemp = ftemp;

        }
        
        public double getFahrenheit ()
        {
            return fahrenheitTemp;
        }

Comments: FROM LINE 97 AND BELOW, THIS IS FLAW CODING.
//        public void setKelvin (double tempInKelvin)
//        {
//            kelvinTemp = tempInKelvin;
//        }
        
        public double getKelvin ()
        {

            kelvinTemp = (5/9 * (fahrenheitTemp - 32) + 273.15);
            return kelvinTemp;
        }
        
//        public void setCelsius (double tempInCelsius)
//        {
//            celsiusTemp = tempInCelsius;
//        }
        
        public double getCelsius ()
        {
            
            celsiusTemp = ((5/9) * (fahrenheitTemp - 32));
            return celsiusTemp;
        }
        
    }
}


//    static void menuDisplay ()
//    {
//        System.out.println("==========================");
//        System.out.println("0. Cancel");
//        System.out.println("1. Fahrenheit");
//        System.out.println("2. Celsius");
//        System.out.println("3. Kelvin");
//        System.out.println("==========================");
//    }
    
//  

//static void choice ()
//    {
//        double fahTemp, kelTemp, celTemp;
//        int choice;
//        
//        Scanner keyboard =  new Scanner(System.in);
//        System.out.print("Enter your choice: ");
//        choice = keyboard.nextInt();
//        
//        if (choice < 0 || choice > 3)
//        {
//            System.out.println("INVALID INPUT FOR CHOICE.\n");
//            
//        }
//        else
//        {
//            switch (choice)
//            {
//                case 1:
//                    
//                    System.out.print("Enter the Fahrenheit temperature: ");
//                    fahTemp = keyboard.nextDouble();
//
//                    Temperature fahrenheit = new Temperature(fahTemp);
//                            
//
//                    System.out.println(fahrenheit.getFahrenheit());
//        
//                    System.out.println("The temperature converted from Fahrenheit to Celsius is " + fahrenheit.getCelsius());
//                    System.out.println("The temperature converted from Fahrenheit to Kelvin is " + fahrenheit.getKelvin());
//                    break;
//                    
//                case 2:
//                    
//                    System.out.print("Enter the Celsius temperature: ");
//                    celTemp = keyboard.nextDouble();
//
//                    Temperature celsius = new Temperature(celTemp);
//
//                    System.out.println(celsius.getCelsius());
//        
//                    System.out.println("The temperature converted from Celsius to Fahrenheit is " + celsius.getFahrenheit());
//                    System.out.println("The temperature converted from Celsius to Kelvin is " + celsius.getKelvin());
//                    break;
//                    
//                case 3:
//                       System.out.print("Enter the Kelvin temperature: ");
//                    kelTemp = keyboard.nextDouble();
//
//                    Temperature kelvin = new Temperature(kelTemp);
//
//                    System.out.println(kelvin.getKelvin());
//        
//                    System.out.println("The temperature converted from Kelvin to Fahrenheit is " + kelvin.getFahrenheit());
//                    System.out.println("The temperature converted from Kelvin to Celsius is " + kelvin.getCelsius());
//                    break;
//                default:
//                    System.out.println("Program ends.\n");
//                    break;
//                    
//        
//            }
//        }
//    }
