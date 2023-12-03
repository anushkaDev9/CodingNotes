# Package & API 
+ package in Java is used to group related classes.<br/>
+ a folder in a file directory.<br/>
**Packages are divided into two categories:**<br/>
Built-in Packages (packages from the Java API)<br/>
User-defined Packages (create your own packages)<br/>
## Built-in Packages
+ Java API is a library of prewritten classes, that are free to use, included in the Java Development Environment.<br/>
<pre>
import package.name.Class;   // Import a single class
import package.name.*;   // Import the whole package
</pre>
# Import a Class
the Scanner class, which is used to get user input, write the following code: <br/>
import java.util.Scanner;
# Import a Package
we used the Scanner class from the java.util package. This package also contains date and time facilities, random-number generator and other utility classes.
o import a whole package, end the sentence with an asterisk sign (*). The following example will import ALL the classes in the java.util package:
import java.util.*;
User-defined Packages<br/>
create your own package, you need to understand that Java uses a file system directory to store them<br/>
![image](https://github.com/ar7937/CodingNotes/assets/83566191/96e21740-3a8e-423a-8a02-b48662787e07)

<pre>
  package mypack;
class MyPackageClass {
  public static void main(String[] args) {
    System.out.println("This is my package!");
  }
}
</pre>
