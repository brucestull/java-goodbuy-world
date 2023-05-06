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

## Resources

* [JDK 17 Documentation](https://docs.oracle.com/en/java/javase/17/)
