# Java Goodbuy, World!

## How to Run the Java Program

1. Change directory into the parent directory of the `src` directory:

    ```powershell
    PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
    ```

1. Inspect directory contents:
    * `tree /f /a`:

        ```powershell
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world> tree /f /a
        Folder PATH listing
        Volume serial number is FEEE-99CC
        C:.
        |   .gitignore
        |   README.md
        |   
        +---.vscode
        |       launch.json
        |       
        \---src
                GoodbuyWorld.java
                
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
        ```

1. Run the Java program:
    * `java .\src\GoodbuyWorld.java`:  

        ```powershell
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world> java .\src\GoodbuyWorld.java
        Goodbuy, World! Enjoy the Sails!
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
        ```

1. Compile the Java program:
    * `javac .\src\GoodbuyWorld.java`:

        ```powershell
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world> javac .\src\GoodbuyWorld.java
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
        ```

1. Inspect directory contents:
    * We now have a `.class` file (`GoodbuyWorld.class`) in the `src` directory.
    * `tree /f /a`:

        ```powershell
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world> tree /f /a
        Folder PATH listing
        Volume serial number is FEEE-99CC
        C:.
        |   .gitignore
        |   README.md
        |   
        +---.vscode
        |       launch.json
        |       
        \---src
                GoodbuyWorld.class
                GoodbuyWorld.java
                
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
        ```

1. Run the compiled Java program, by telling Java where to look for the `.class` file:
    * `java -cp src GoodbuyWorld`

        --OR--
    * `java -cp .\src GoodbuyWorld`

        --OR--
    * `java -cp src\ GoodbuyWorld`

        ```powershell
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world> java -cp src GoodbuyWorld
        Goodbuy, World! Enjoy the Sails!
        PS C:\Users\FlynntKnapp\Programming\java-goodbuy-world>
        ```

## Running the Java Program

### Get Help on the `java` Command

* `java --help` or `java -h` - Get help on the `java` command.

### Run the Java Program without Compiling

* `java .\src\GoodbuyWorld.java`

### Compile then Run the Java Program

1. Compile the Java program:
    * `javac .\src\GoodbuyWorld.java`
1. Run the compiled program using one of the following commands (among others):
    * `java -cp src GoodbuyWorld`
    * `java -cp .\src GoodbuyWorld`
    * `java -cp src\ GoodbuyWorld`
    * `java -classpath src\ GoodbuyWorld`
    * `java --class-path src\ GoodbuyWorld`

* Here are some options/flags that tell Java where to look for the `.class` file (From java --help):

    ```powershell
    -cp <class search path of directories and zip/jar files>
    ```

    ```powershell
    -classpath <class search path of directories and zip/jar files>
    ```

    ```powershell
    --class-path <class search path of directories and zip/jar files>
                    A ; separated list of directories, JAR archives,
                    and ZIP archives to search for class files.
    ```

## Resources

* [JDK 17 Documentation](https://docs.oracle.com/en/java/javase/17/)
