# Your First Java Program

Now we are going to create the obligatory `Hello World` code like we do every time we learn a new language.

> Create this sample program in a file named HelloWorld.java

```java
class HelloWorld {
  public static void main(String args[]) {
    System.out.println("Hello World!");
  }
}
```

~~~python
print("Hello World!")
~~~

Note: You can select Python in the top part of the screen to see the rough equivalence of the code in Python.

## Compiling and Running Program

Now that you've created the template, you can see what output it produces.

> You can run it by compiling it first

```shell
javac HelloWorld.java && java HelloWorld
```