# Object Oriented Programming

## the idea is to marry state and behavior 

```vb
Dim myName as String
Set myName = "Warren"

myname = UCase(myName)
```

```csharp
var myName = "Warren";
myName = myName.ToUpper();

```

## Ojects have:

### state
Variables that the object "owns"
in .net state is in class level variables 'Fields'

### Behavior
code that cam be invoked that has something to do with the data (state) owned by that object 
in .net the behavior is methods:

Constructors 

Properties

Events

## Example 

I have an object that represents a bank account 
### state 
Bank Account have a current balance 
```csharp
public class BankAccount
{
    private decimal _currentBalance = 0;
}
```
### behaviors
we can add subtract or view balance 
```csharp
public class BankAccount
{
    private decimal _currentBalance = 0;

public void Deposit(decimal amount)
{
    _currentBalance += amount;
}
public void Withdraw(decimal amount)
{
    _currentBalance -= amount;
}
public void View()
{
    console.writeline($"Your Balance is {_currentBalance}");
}

}
```