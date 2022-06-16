## Can't Launch .jar File
You can't launch the .jar file by double-clicking. This means your Java installation is not valid.
### Verifying Java is installed:
You can verify that Java is installed by opening a command terminal and running the command ```java -version```.
You should see a message summarizing the active Java version. If running that command results in an error message saying that the java command is not
recognized (or similar), then your Java installation is invalid, and you should run the 64-bit installer found [here](https://java.com/en/download/manual.jsp).
### Using the right version:
It may be that you have the correct version of Java installed, but that a different one is being used to launch the application. When you run the above command,
you should see a version of java 1.8.0. The one I provide a link to is version 1.8.0_331. If you don't see a 1.8.0 version when running the command,
it means that your system is configured to use the wrong version of Java for this program. You can either manually run the program using the correct version with a command (or set up a .bat file or equivelant to do that).

You should also be able to associate .jar files with a specific version of Java so that they are launched with that version when clicked, but I can't figure out an easy way of doing that, so [here's](https://stackoverflow.com/questions/48380001/executable-jar-not-running-windows-10) a link to an obscure StackExchange post instead.

All my devices run a version of Windows, so the rest of this section will be Windows-specific advice, but I think these concepts can be easily adapted to other operating systems.
#### By command or .bat file:
On Windows, you can run GCSD with a command like this: ```"C:\Program Files\Java\jre1.8.0_331\bin\java.exe" -jar GraphingCalculatorSD-v1.28.1.jar```
(Note that to run the command, you must navigate the cmd terminal to the directory containing the GraphingCalculatorSD jar.)

The first term ("C:\...\java.exe") is the path to the proper Java installation. By default, this is located in C:\Program Files\Java\\\<JREVersion>\bin\java.exe.

The second and third terms (-jar GraphingCalculator...jar) specify that Java should be used to run the given .jar file.

If you want to use this command in PowerShell, you need to prefix the command with "& " in order for the string to be executed. E.g: ```& "C:\Program Files\Java\jre1.8.0_331\bin\java.exe" -jar GraphingCalculatorSD-v1.28.1.jar```

You can then create a new .bat file in the same folder as GCSD, and place the first command within. It will then be run when you double-click the .bat file. [Here](launch.bat) is a .bat file you can download and use as a template. Note that this is a somewhat imperfect solution, in that when you update GCSD, you'll need to update the version number in the .bat file too, in order to target the new program jar.

#### [Back](problems.md)
