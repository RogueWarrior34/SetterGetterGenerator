
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

5. The tool will analyze the class and generate the necessary setter and getter methods, as well as a default constructor.

6. The generated code will be printed to the console, and you can copy and paste it into your Java class.

## Example
Suppose you have a Java class named EmployeeDTO as 
```
public class EmployeeDTO
{
private String employeeId;
private String name;
private int designationCode;
private Date dateOfBirth;
private char gender;
private boolean isIndian;
private BigDecimal basicSalary;
private String panNumber;
private String aadharCardNumber;
}
```
. Running the tool as follows in the same directory as your class:

```
java -classpath path\SetterGetterGenerator\dist\rwcommon.jar com.rogue.util.SetterGetterGenerator EmployeeDTO
```
will generate the following code and will save it in a file named as *tmp.tmp*:

```
public class EmployeeDTO
{
private String employeeId;
private String name;
private int designationCode;
private Date dateOfBirth;
private char gender;
private boolean isIndian;
private BigDecimal basicSalary;
private String panNumber;
private String aadharCardNumber;

public EmployeeDTO()
{
this.employeeId="";
this.name="";
this.designationCode=0;
this.dateOfBirth=null;
this.gender=' ';
this.isIndian=false;
this.basicSalary=null;
this.panNumber="";
this.aadharCardNumber="";
}
public void setEmployeeId(java.lang.String employeeId)
{
this.employeeId=employeeId;
}
public java.lang.String getEmployeeId()
{
return this.employeeId;
}
public void setName(java.lang.String name)
{
this.name=name;
}
public java.lang.String getName()
{
return this.name;
}
public void setDesignationCode(int designationCode)
{
this.designationCode=designationCode;
}
public int getDesignationCode()
{
return this.designationCode;
}
public void setDateOfBirth(java.util.Date dateOfBirth)
{
this.dateOfBirth=dateOfBirth;
}
public java.util.Date getDateOfBirth()
{
return this.dateOfBirth;
}
public void setGender(GENDER gender)
{
if(gender==GENDER.MALE) this.gender='M';
else this.gender='F';
}
public char getGender()
{
return this.gender;
}
public void setIsIndian(boolean isIndian)
{
this.isIndian=isIndian;
}
public boolean getIsIndian()
{
return this.isIndian;
}
public void setBasicSalary(java.math.BigDecimal basicSalary)
{
this.basicSalary=basicSalary;
}
public java.math.BigDecimal getBasicSalary()
{
return this.basicSalary;
}
public void setPANNumber(java.lang.String panNumber)
{
this.panNumber=panNumber;
}
public java.lang.String getPANNumber()
{
return this.panNumber;
}
public void setAadharCardNumber(java.lang.String aadharCardNumber)
{
this.aadharCardNumber=aadharCardNumber;
}
public java.lang.String getAadharCardNumber()
{
return this.aadharCardNumber;
}
public int hashCode()
{
return this.employeeId.toUpperCase().hashCode();
}
public boolean equals(Object other)
{
if(!(other instanceof EmployeeDTOInterface)) return false;
EmployeeDTOInterface employeeDTO=(EmployeeDTOInterface) other;
return this.employeeId.equalsIgnoreCase(employeeDTO.getEmployeeId());
}
public int compareTo(EmployeeDTOInterface employeeDTO)
{
return this.employeeId.compareToIgnoreCase(employeeDTO.getEmployeeId());
}
}
```

## Source Files
-Source files are in *SetterGetterGenerator\src\com\rogue\util*
## Class files
-Class files are in *SetterGetterGenerator\classes*

## Contribution
If you would like to contribute to this project or report issues, please feel free to open an issue or create a pull request on the [SetterGetterGeenerator repository](https://github.com/RogueWarrior34/SetterGetterGenerator/blob/main/LICENSE).

## License
This Java Setter/Getter Generator is open-source software released under the [MIT License](https://github.com/RogueWarrior34/SetterGetterGenerator/blob/main/LICENSE). Feel free to use and modify it in your projects.
