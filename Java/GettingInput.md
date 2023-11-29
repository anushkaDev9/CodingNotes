# Scanner
Scanner class is used to get user input, and it is found in the java.util package.
<pre>
  import java.util.Scanner;  // Import the Scanner class

class Main {
  public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);  // Create a Scanner object
    System.out.println("Enter username");

    String userName = myObj.nextLine();  // Read user input
    System.out.println("Username is: " + userName);  // Output user input
  }
}
</pre>
+ nextBoolean()-Reads a boolean value from the user<br/>
+ nextByte()-Reads a byte value from the user<br/>
+ nextDouble()-Reads a double value from the user<br/>
+ nextFloat()-Reads a float value from the user<br/>
+ nextInt()-Reads a int value from the user<br/>
+ nextLine()-Reads a String value from the user<br/>
+ nextLong()-Reads a long value from the user<br/>
+ nextShort()-Reads a short value from the user.<br/>
scan.nextLine(); // Skip the newline character after the double
