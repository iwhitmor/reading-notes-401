# Exception Handling

## [Debugging for absolute beginners](https://docs.microsoft.com/en-us/visualstudio/debugger/debugging-absolute-beginners?view=vs-2019&tabs=csharp)

* Debugging means to runy our code step by step using a debugger tool to find the exact spot you made a mistake

* Using a debugger is a skill that takes time learn, but is very necessary and becomes a fundamental task for all software developers

* Steps to using the debugger:

  * Clarify the problem

    * What did you expect your code to do?

    * What happened instead?

  * Examine your assumptions

    * Check all the small details

      * Are you using the right API? Using it correctly?

      * Check for typos, other details, etc...

  * Step through your code using the debugging tool to find where the problem occurred

    * Set a breakpoint in your code in Visual Studio

      * A breakpoint indicates where Visual Studio should pause your running code so you can see what is going on

## [Try/Catch Blocks](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions)

* Place any code statements that might raise or throw an exception in a try block, and place statements used to handle the exception or exceptions in one or more catch blocks below the try block. Each catch block includes the exception type and can contain additional statements needed to handle that exception type.

* The Common Language Runtime (CLR) catches exceptions not handled by catch blocks. If an exception is caught by the CLR, one of the following results may occur depending on your CLR configuration:

  * Debugger box appears 

  * The program stops execution and box with execution info appears

  * An error prints out

## [Exception Handling](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/statement-keywords)

* Statements are program instructions. Except as described in the topics referenced in the following table, statements are executed in sequence. The following table lists the C# statement keywords. For more information about statements that are not expressed with any keyword, see Statements.

### Additional Resources

* Information taken from links provided above
