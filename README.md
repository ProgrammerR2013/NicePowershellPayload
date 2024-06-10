# NicePowershellPayload
EDUCATIONAL PURPOSES ONLY

This is a more advanced payload developed in PowerShell, and it's pretty useful for penetration testing tasks on Windows OS mainframes. 

This PowerShell script dynamically compiles C# code contained in the $code variable, which includes a class Cat inside the Nyan namespace. This class has a method Run().

Inside the Run() method:

1. It creates a WebClient to download a base64-encoded string from a specific URL.
2. It decodes the downloaded string into a byte array and loads it as an assembly into the current AppDomain.
3. It retrieves the entry point (main method) of the loaded assembly.
4. It creates an instance of the class containing the entry point method.
5. It invokes the entry point method with any necessary parameters.
6. The commented-out portion seems to be an attempt to run the assembly download and execution process in a separate thread, but it's currently disabled.

Finally, it compiles and runs the code by creating an instance of the Cat class and invoking its Run() method.
Erase the comment signs if you want to enable it to run the execution process in a different thread.

This is a pretty advanced code and I haven't written any more complex payloads, but I will in the future!
