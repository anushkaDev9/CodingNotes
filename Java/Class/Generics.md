# Generics 
allows us to create a single class, interface, and method that can be used with different types of data (objects).<br/>
create a class that can be used with any type of data. Such a class is known as Generics Class.<br/>
<pre>
  public class App {
	public static void main(String[] args) {
		ArrayList list=new ArrayList();
      list.add("apple");
      list.add("grapes");
      String fruit=(String)list.get(0);
     /* System.out.println(list.get(1));
      ArrayList<String> fruits=n  */
      ArrayList <String> animals=new ArrayList<>();
      animals.add("apples");
      animals.add("grapes");
      animals.add("banana");
      String ani=animals.get(0);
      System.out.println(animals.get(2));
      HashMap<Integer,String> maps=new HashMap<Integer,String>();
	}
}
</pre>
Here, T used inside the angle bracket <> indicates the type parameter. Inside the Main class, we have created two objects of GenericsClass
intObj - Here, the type parameter T is replaced by Integer. Now, the GenericsClass works with integer data.
stringObj - Here, the type parameter T is replaced by String. Now, the GenericsClass works with string data.
