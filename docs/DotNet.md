# DotNet Over View

![Dotnet Overview](/img/dotnet.excalidraw.svg)

## What is it??

A platform for writing and running software from M$ -- released in 2002. -- Originally Java antithesis 

## dotnet running 

THE **Common Language Runtime (CLR)** is a managed runtime for your application. Your app is partially compiled to intermediate language and then just in time compiled to run at runtime.

>.NET compile to IL code

.NET compile to assembly
 - Assembly has the IL code 
 - Assembly as a database of the Types

Each **Project** compiles into an assembly
Each **Solution** is a workspace that can have more than one project

**CODE**
Console.WriteLine("Welcome to the Application!");




Console.Write("Enter your name: ");
string? name = Console.ReadLine();



Console.Write("What is your Age?");



string? ageAsString = Console.ReadLine();
int age = 0;
try
{
    age = int.Parse(ageAsString);
}
catch (FormatException)
{



   Console.WriteLine("Enter a number for your age, jerk!");
    throw;
}



if (name == null)
{
    Console.WriteLine("Come on! Tell me your name!");
}
else
{



   Console.WriteLine($"Welcome to the application, {name}! Good to see you! You are {age} years old!");
}