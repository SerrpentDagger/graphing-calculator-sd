## Can't Launch .jar File
You can't launch the .jar file by double-clicking. This means your Java installation is not valid.
### Verifying Java is installed:
You can verify that Java is installed by opening a command terminal and running the command ```java -version```.
You should see a message summarizing the active Java version. If running that command results in an error message saying that the java command is not
recognized (or similar), then your Java installation is invalid, and you should run the installer found [here](https://java.com/en/download/manual.jsp).
### Using the right version:
It may be that you have the correct version of Java installed, but that a different one is being used to launch the application. When you run the above command,
you should see a version of java 1.8.0. The one I provide a link to on the home page is version 1.8.0_331. If you don't see a 1.8.0 version when running the command,
it means that your system is configured to use the wrong version of Java for this program. You can either manually run the program using the correct version with a command (or set up a .bat file or equivelant to do that), or configure your JAVA_HOME or JRE_HOME environment variables to point to the right Java installation (that is a system-wide change that affects other programs).

#### [Back](problems.md)
