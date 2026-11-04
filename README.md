# RNG

A small JavaFX desktop app that generates a random whole number between 0 and an upper limit you type in. It was an early GUI practice exercise: a text field for the limit, a large Generate button, and a read-only field that shows the result.

## Stack

- Java with JavaFX (no build tool; plain source files)
- `java.util.Random`

## Running

There is no Maven or Gradle file, so compile and run with a JavaFX SDK on the module path. Replace `<path-to-javafx-sdk>` with the location of your JavaFX SDK.

```
javac --module-path <path-to-javafx-sdk>/lib --add-modules javafx.controls *.java
java  --module-path <path-to-javafx-sdk>/lib --add-modules javafx.controls Window
```

Enter a positive integer in the small text box and click Generate.

## Project layout

- `Window.java` - JavaFX application, layout and button handler
- `Generator.java` - reads the limit and produces the random number

## Status

Small learning project, not under development. Input validation is basic and there are no tests.
