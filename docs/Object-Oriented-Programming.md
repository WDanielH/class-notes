## To be OOP:

Support:
- Encapsulation
- Polymorphism
- Inheritence
- Runtime Type Inspection

:::note what is OOP by Alan Kay
OOP means only messaging, local retention and protection and hiding
of state process, and extreme late binding of all things.
:::

## Objects Have:

### state 
Variables that the object "owns"

### behavior 
code that can be invoked that has something to do with state 

### properties in C#
1. Properties *imply* no computation
2. If you throw an exception on a property set or get you are a jerk
3. Once a property is set, then getting that property a million times in the row should return the same value


## Example
I have an object that represents a bank account 

### State
Bank Accounts have a balance 

### vary behavior based on parameters

```csharp
account.Deposit(20);
//compared to
account.Deposit(100):
```

### vary behavior based on the object 

```csharp
acount.Type = AccountTypes.Gold
account.Deposit(20);

account.Deposit(100):
```

### vary behavior by typ e

```csharp
var account = new BankAccount();
account.Deposit(100);

```

```csharp
var account = new GoldAccount();
account.Deposit(100);

```