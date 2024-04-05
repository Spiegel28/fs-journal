# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > allows a class to inherit another classes properties 

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > when a class inherits from another class, it inherits both the accessible members (fields, properties, methods, and events) and the accessibility level of those members from the base class. 

3. How does ***accessibility*** affect inheritance?

  > determines which members of a class are visible and accessible from outside the class or from derived classes. It plays a crucial role in inheritance as it determines which members of a base class are inherited by derived classes and how they can be accessed.

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > constraints are used to enforce integrity and relationships in a relational database, the primary key uniquely identifies rows within a table, whereas the foreign key establishes relationships between tables by referencing the primary key or unique constraint of another table.







5. What is an ***alias***?

  > alternative name given to an entity

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > SELECT patient.*
FROM patients patient
 JOIN patient_doctors pd ON patient.id = pd.patientId
WHERE pd.doctorId = doctor_id;
