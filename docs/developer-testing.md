## Developer Testing

developers are writing the tests as they write the code. 

## Quality 

# Internal Quality 
You wrote the code, it is *loosely coupled, highly cohesive* it is **adaptable** because like Thanos, **change** is ***Inevitable***

# External Quality 
**Most important --  The code does what it is supposed to do** -- You met the business requirements.

>A paragraph
*italics*
**bold**
***superbold***
>
## Feedback Loops 
We want to see what it going on, *good* **or** *bad*

## Inner Loop
All that stuff that happens under our fingers in our devlopment enviornment. Instant feedback.

## Outer Loop
That the stuff that happens after we push our code to the source and our build pipeline takes over -- much slower feedback loop 

## Four Levels of Testing

# static
things the language/compiler is stopping us from doing -- super *inner loop* 

# unit testing 
testing a functional unit of code in isolation from the other code. In C# that is usually a single method. also *super inner loop*  -- shouldnt be touching databases or networks or filesystems 

# Integration Testing
Any time we test two or more functional units of code together. Seeing how our code integrates with other code 

# End to End Testing 

Often in the form of smoke tests -- before you put the code in front of users, you have some automated tests to verify it is ready. 

this is usually the perview of software testers. 

## test driven development 
A form of test first implemented as a design philosophy -- more about designing code than development

If you do **TDD**

# *red* 
Starting with a meaningfully failing test.

# *green* 
Write just enough code to make the test pass. It doesn't need to be "GOOD" just make the test pass.
This ensures that you understand the problem and how to solve it before you worry about how *best* to do it.

# *refactor* 
After the test is passing, make it good. Look for duplication, look for latent abstractions

# *commit (sometimes)*

