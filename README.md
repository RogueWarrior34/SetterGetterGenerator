
# Java Setter/Getter Generator

## Introduction
The Java Setter/Getter Generator is a tool that simplifies the process of generating default constructors, setter, and getter methods for a Java class. This tool can save you a significant amount of time when creating and maintaining Java classes, as it automatically generates code for accessing and modifying class attributes.

## Features
1. Default Constructor Generation: Quickly generate a default constructor for your class, initializing all fields to their default values.

2. Setter Generation: Generate setter methods for each field, allowing you to set the values of class attributes.

3. Getter Generation: Generate getter methods for each field, enabling you to retrieve the values of class attributes.

## Usage
1. Clone this repository to your local machine or download the source code.

2. Build your project using your preferred Java development environment, or compile the source code manually.

3. Run the Setter/Getter Generator with the following command:
   
        java -classpath path\SetterGetterGenerator\dist\rwcommon.jar com.rogue.util.SetterGetterGenerator YourClassName
   Replace YourClassName with the name of the Java class for which you want to generate setters, getters, and a default constructor.

4. The tool will analyze the class and generate the necessary setter and getter methods, as well as a default constructor.

5. The generated code will be printed to the console, and you can copy and paste it into your Java class.

## Source Files
-Source files are in *SetterGetterGenerator\src\com\rogue\util\SetterGetterGenerator.java*
## Class files
-Class files are in *SetterGetterGenerator\classes*

## Contribution
If you would like to contribute to this project or report issues, please feel free to open an issue or create a pull request on the [SetterGetterGeenerator repository](https://github.com/RogueWarrior34/SetterGetterGenerator/blob/main/LICENSE).

## License
This Java Setter/Getter Generator is open-source software released under the [MIT License](https://github.com/RogueWarrior34/SetterGetterGenerator/blob/main/LICENSE). Feel free to use and modify it in your projects.
