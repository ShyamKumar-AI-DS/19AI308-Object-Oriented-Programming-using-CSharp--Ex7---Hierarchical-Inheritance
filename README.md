# Ex7---Hierarchical-Inheritance

## AIM:
To write a C# program to implement heirarchical inheritance for the following problem statement:  All the vehicles need Tyres on their wheels. 
So, the manufacturer designs their vehicle as they want and import Tyre from its base class and fit it into Wheels. 
They don’t need to design Tyre all the time. Once they designed the model and use it various times. 
Aim is to create a Scooter and Car vehicle where the Tyre is being inherited from vehicle class.

## ALGORITHM:
### Step 1:
Define a base class 'Vehicle' with a method 'tyre' to describe tyres.

### Step 2:
Create a 'Scooter' class inheriting 'Vehicle', with a method 'Display' and 'tyres'.

### Step 3:
Implement 'Display' to show class type and call base 'tyre'.

### Step 4:
Similarly, make a 'Car' class inheriting 'Vehicle', with a 'Display' method.

### Step 5:
Instantiate Car' and 'Scooter', call 'Display' with respective tyre counts.

## PROGRAM:
```
Developed by : Shyam Kumar A
Reg No:   212221230098

```
```c#
using System;
namespace inheritance
{
    class Program
    {
        static void Main(string[] args)
        {
            Scooter scooter = new Scooter();
            Car car = new Car();
        
        
            Console.WriteLine("Scooter started:");
            scooter.display();
        
            Console.WriteLine("\nCar started:");
            car.display();
  
        }
    }
    //Creating Base Class
    public class Vehicle
    {
        public void tyre()
        {
            Console.WriteLine("It is a tubeless tyre");
        }
    }
    //Creating Child Class
    class Scooter : Vehicle
    {
        public void display() 
        {
            base.tyre();
            Console.WriteLine("It is a scooter class");
        }
    }
    //Creating Child Class
    class Car : Vehicle
    {
        public  void display() 
        {
            base.tyre();
            Console.WriteLine("It is a car class");
        }
    }
}


```
## OUTPUT:
![image](https://github.com/ShyamKumar-AI-DS/19AI308-Object-Oriented-Programming-using-CSharp--Ex7---Hierarchical-Inheritance/assets/93427182/26250894-3160-409f-80fb-b2bf4bb3afb6)

## RESULT:
Thus, the C# program to implement hierarchical inheritance is verified and executed successfully.

