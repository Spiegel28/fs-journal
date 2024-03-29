# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > a namespace is a container that holds a set of identifiers, such as functions, variables, classes, etc., and provides a way to organize and encapsulate them to avoid name conflicts and to manage the complexity of large codebases.

02. What is the difference between a `class` and an `interface`?

  > A class is a concrete implementation that defines both data and behavior.
An interface is a contract that defines a set of methods without providing implementations, allowing multiple classes to implement the same interface with their own implementations.

03. What is the method that returns an instance of a class, yet it has no return type?

  > Constructor 

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > public 

06. In the Car example what is `string` an indication of?

  > a string value 

07. In the Car example what is `abstract` preventing?

  > prevents editing the code 

08. In a SQL table, what is the difference between information in a row and information in a column?

  > rows represent individual data entries, while columns represent the attributes or fields associated with those data entries. Together, rows and columns organize the structured data within a SQL table.

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE characters (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    age VARCHAR(50),
    description VARCHAR(1000)
);

10. In SQL how can you query more than a single table? Provide an example.

  > A JOIN 
  
  SELECT characters.name, characters.age, character_details.description
FROM characters
JOIN character_details ON characters.id = character_details.id;
