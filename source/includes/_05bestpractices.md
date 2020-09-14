# Best Practices & Common Pitfalls

## Remember to use semicolon (;)

Different with Python, in Java you must put semicolon after you declare something. Your code will be eror if you leave something without put semicolon.

> Example without semicolon

~~~java
public class Semicolon {
    public static void main(String[] args) {
        System.out.print("What's wrong??")
		System.out.print("Ohh there are no semicolon at there")
    }
}
~~~

> Example with semicolon

~~~java
public class Semicolon {
    public static void main(String[] args) {
        System.out.print("Like this??");
		System.out.print("Ohh yes this code already completed with semicolon");
    }
}
~~~

## Use File Name for Public Class Name

Your public class name must be the same with your file name or your code will get error while you compile it.

> Wrong public class name for Java file named 'Fasilkom'

~~~java
public class Pacil {
    public static void main(String[] args) {
        System.out.print("My class name is wrong");
    }
}
~~~

> correct public class name for Java file named 'Fasilkom'

~~~java
public class Fasilkom {
    public static void main(String[] args) {
        System.out.print("Ahh this class name sounds right");
    }
}
~~~

## Use Lower Case for 'main' Method

Your program on Java must have a main method. Remember that you must type it in lower case only. The compiler couldn't find your main method if you use uppercase. (It's case sensitive)

> Upper case 'Main'

~~~java
public class Upper {
    public static void Main(String[] args) {
        System.out.print("Wow, my main method looks wrong");
        System.out.print("Let we try to compile!");
    }
}
~~~

> Lower case 'main'

~~~java
public class Lower {
    public static void main(String[] args) {
        System.out.print("Hmm, maybe may main method must like this");
        System.out.print("Let's try it!");
    }
}
~~~

## There is Only One Main Method

You could only have one main method for your Java program. Your compiler will be confused if you have more than one. Be loyal with your one.

> More than one main method

~~~java
public class Two {
    public static void main(String[] args) {
        System.out.print("You're my first!!");
    }

    public static void main(String[] args) {
        System.out.print("And you're my first too in alternate world");
    }
}
~~~

> Only one main method

~~~java
public class One {
    public static void main(String[] args) {
        System.out.print("You're my one and only!!");
    }
}
~~~

## Remember to Declare Variable Type

Again, different with Python, in Java you couldn't create a variable without declare what is your variable type.

> No variable type

~~~java
public class NoType {
    public static void main(String[] args) {
        naruto = "RASENGANN!!!";
        maung = 2019;
        revolution = 4.0;

        System.out.print("When the enemies almost kill you, just go ahead and said, " + naruto);
        System.out.print("Maung is the name of Fasilkom year of " + maung);
        System.out.print("Right now we go through industry revolution " + revolution);
    }
}
~~~

> Using variable type

~~~java
public class NoType {
    public static void main(String[] args) {
        String naruto = "RASENGANN!!!";
        int maung = 2019;
        double revolution = 4.0;

        System.out.print("When the enemies almost kill you, just go ahead and said, " + naruto);
        System.out.print("Maung is the name of Fasilkom year of " + maung);
        System.out.print("Right now we go through industry revolution " + revolution);
    }
}
~~~