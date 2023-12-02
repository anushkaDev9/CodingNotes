# Date & Time
+ does not have a built-in Date class, but we can import the java.time package <br/>
![image](https://github.com/ar7937/CodingNotes/assets/83566191/9bd68614-55b8-4b69-8424-112bfb126ca5)
## Current Date 
import the java.time.LocalDate class, and use its now()<br/>
<pre>
  import java.time.LocalDate; // import the LocalDate class
public class Main {
  public static void main(String[] args) {
    LocalDate myObj = LocalDate.now(); // Create a date object
    System.out.println(myObj); // Display the current date
  }
}
</pre>
## Current Time 
import the java.time.LocalTime class, and use its now() method:
<pre>
  import java.time.LocalTime; // import the LocalTime class

public class Main {
  public static void main(String[] args) {
    LocalTime myObj = LocalTime.now();
    System.out.println(myObj);
  }
}
</pre>
# Formatting Date and Time
+ DateTimeFormatter class with the ofPattern() method in the same package to format or parse date-time objects<br/>
 <pre>
   import java.time.LocalDateTime; // Import the LocalDateTime class
import java.time.format.DateTimeFormatter; // Import the DateTimeFormatter class

public class Main {
  public static void main(String[] args) {
    LocalDateTime myDateObj = LocalDateTime.now();
    System.out.println("Before formatting: " + myDateObj);
    DateTimeFormatter myFormatObj = DateTimeFormatter.ofPattern("dd-MM-yyyy HH:mm:ss");
    String formattedDate = myDateObj.format(myFormatObj);
    System.out.println("After formatting: " + formattedDate);
  }
}
 </pre>
 ![image](https://github.com/ar7937/CodingNotes/assets/83566191/eae3e903-5b52-4006-8e25-34525d55d754)
