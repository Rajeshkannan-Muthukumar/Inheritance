# Inheritance

## Aim:
To write a C# program to print some messages using hierarchical inheritance.


## Algorithm:

### step 1:
Create a base class.

### step 2:
Create two child class.

### step 3:
Create a constructor in the base class and print a message.

### step 4:
create a function in child class to print a message.
## Program:
```

using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Constructor tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("tyre");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Constructor scooter");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("scooter");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Constructor car");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("car");
        }
    }

    public class Program
    {
        public static void Main(string[] args)
        {
            car c = new car();
            scooter s = new scooter();
            c.Display();
            s.Display();
        }
    }
}


```
## Output:
![OP](1.png)

## Result

C# program to print some messages using hierarchical inheritance is implemented successfully.

