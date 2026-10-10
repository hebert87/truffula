    # Truffula Notes
    As part of Wave 0, please fill out notes for each of the below files. They are in the order I recommend you go through them. A few bullet points for each file is enough. You don't need to have a perfect understanding of everything, but you should work to gain an idea of how the project is structured and what you'll need to implement. Note that there are programming techniques used here that we have not covered in class! You will need to do some light research around things like enums and and `java.io.File`.

    PLEASE MAKE FREQUENT COMMITS AS YOU FILL OUT THIS FILE.

## App.java
- It looks like this is where the program starts because it contains the main method.
-String[] args receives the arguments, such as -h, -nc, and the directory path.
-TruffulaOptions will determine what to do with the arguments, such as whether to show hidden files, turn off colors, and which directory to print.
-TruffulaPrinter will use those options to print the directory tree by calling printTree().
Question: What happens if an argument is invalid or the directory doesn't exist? How will the program handle it?

## ConsoleColor.java
-This file uses an enum called ConsoleColor to list the colors that can be used in the terminal.
-Each color, like GREEN, RED, and BLUE, has an ANSI escape code stored as a String. -These codes tell the terminal what color to display.
-The constructor takes the color code and stores it in the code field.
-The getCode() method returns the color code, and toString() also returns the code as a string.
- RESET is used to return the terminal text color to its default.
Question: How does ColorPrinter use these color codes when printing the directory tree?

## ColorPrinter.java / ColorPrinterTest.java

## TruffulaOptions.java / TruffulaOptionsTest.java

## TruffulaPrinter.java / TruffulaPrinterTest.java

## AlphabeticalFileSorter.java