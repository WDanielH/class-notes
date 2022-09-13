# C# Types

```csharp
public class Program
{
    public static void Main(string[] args)
    {
        Console.Writeline("Hello Worlds!")
    }
}
```
Notes:
The CTS has two broad families of types in .NET, these are the *first-class-citizens* of .net. "Things a variable can refer to"

## Value Types 
 - memory managed automatically and their life and scope is predictable. The value lives on the stack. it is removed from the stack with the variable goes out of scope.
 Value types are structs in C#

## Reference Types
- Reference types have values that live on the "managed" heap.
The stack has a reference to the value on the heap
The memory is allocated automatically and deallocated using a generational garbage collector 