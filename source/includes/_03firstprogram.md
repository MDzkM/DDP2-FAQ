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

> If you want to know, this is the roughly equivalent code in Python

~~~python
print("Hello World!")
~~~



## Compiling and Running Program

Now that you've created the template, you can see what output it produces.

> You can run it by compiling it first

```shell
javac HelloWorld.java && java HelloWorld
```