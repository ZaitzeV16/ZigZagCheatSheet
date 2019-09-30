# W03 - D02 - File I/O and Exception Handling
***made by [Vivi](https://github.com/bodavivi)***

- [Exception Handling](#exception-handling)
- [File I/O](#file-io)
    - [Path](#path)
    - [Reading Files](#reading-files)
    - [Writing Files](#writing-files)

## Exception Handling
> + If the code in `try` doesn’t work, `catch` starts.
> + several `catch` can belong to one `try`
>   + they work like `if` – if the first `catch` comes true, the following ones won’t run

`catch()` contains the error which can happen
+ `Exception` -  covers all errors, but is not too informative
+ `ArithmeticException` – calculation error (like divide with 0)
+ `IOException` – errors related to file manipulation (like you wanna read a path which doesn’t exist)
+ etc...

> Checked exceptions
> + they are checked before the program running, 
and if they are wrong, the program doesn’t run
> + it’s a checked exception to run the codes with File manipulating in `try`

```java
try {
  // Block of code to try
}
catch(Exception exceptionName) {
  //  Block of code to handle errors
  exceptionName.printStackTrace(); // to print out the error msg
}
catch(OtherException exceptionName) {
  //  Block of code to handle errors
  // `exceptionName` is a name you choose for the exception
  // `exceptionName.printStackTrace()` prints the error out (not required)
  exceptionName.printStackTrace();
}
// .
// .
// .
finally{
  //  finally always runs (doesn’t matter if there was error or not)
}
```

****

## File I/O
### Path
> ***The path of the file.***
> + ***relative***: start from the current directory (like Day-01)
> + ***absolute***: from root directory

```java
Path pathName = Paths.get("filename.type");
```

****

### Reading Files
> Read the file (called pathname in this case) line by line;
and put it in a list (called name in this case). 

```java
List<String> name = Files.readAllLines(pathName);
```

****

### Writing Files
> Write the lines from list called name, to a file which is in the `pathname` path.

```java
Files.write(pathname, name);
```
