WEEK 2 (SPRING CORE MAVEN)


# Library Management System

This project demonstrates a basic library management system using the Spring Framework  , lets see exercise ……
Exercise 1: Configuring a Basic Spring Application
 Steps:

1. 1st I have Created  a Maven project named `LibraryManagement`. Then  added Spring Core dependencies in the `pom.xml` file.

2. In Step 2 , I have Created an XML configuration file named `applicationContext.xml` in the `src/main/resources` directory and also defined beans for `BookService` and `BookRepository` in the XML file.

3. In step 3 , I also have created a package `com.library.service` and add a class `BookService` and created a package `com.library.repository` and add a class `BookRepository`.

4. In step4 , Here is the run application part. Here I created a main class to load the Spring context and test the configuration.

 Exercise 2: Implementing Dependency Injection
  Steps:

1. Step 1 is, Modifying the XML Configuration:
   -Here we have to 1st update `applicationContext.xml` to wire `BookRepository` into `BookService`.

2. Step 2,The we have to ensure that `BookService` class has a setter method for `BookRepository`.

3. Step 3 . Here is the Test the Configuration ,
  We have to Run the `LibraryManagementApplication` main class to verify the dependency injection.

 Exercise 3: Implementing Logging with Spring AOP

 Steps:

1.	1st, we have to  update `pom.xml` to include Spring AOP dependency.

2.	Step 2 , we have to  create a package `com.library.aspect` and add a class `LoggingAspect` with a method to log execution times.

3. Step 3, The, we have to update `applicationContext.xml` to enable AspectJ support and register the aspect.

4. Here is The Test the Aspect:
   -we have to run the `LibraryManagementApplication` main class and observe the console for log messages indicating method execution times.

Exercise 4: Creating and Configuring a Maven Project

 Steps:

1.	we have created a new Maven project named `LibraryManagement`.

2.   The I has  included dependencies for Spring Context, Spring AOP, and Spring WebMVC.

2.	After that , I  configured the Maven Compiler Plugin for Java version 1.8 in the `pom.xml` file.

Exercise 5: Configuring the Spring IoC Container
Steps:

1.	 1st we have to  Create an XML configuration file named `applicationContext.xml` in the `src/main/resources` directory and then define beans for `BookService` and `BookRepository` in the XML file.

2.   Then , I ensure that the `BookService` class has a setter method for `BookRepository`.

2.	In last , I have created  a main class to load the Spring context and test the configuration.

 Exercise 6: Configuring Beans with Annotations

Steps:

1.	I  Updated `applicationContext.xml` to include component scanning for the `com.library` package.

2.   – I had to  Use `@Service` annotation for the `BookService` class and `@Repository` annotation for the `BookRepository` class.

3. Here is the test part , to run the `LibraryManagementApplication` main class to verify the annotation-based configuration.


Exercise 7: Implementing Constructor and Setter Injection
Steps:

1.	Here I have updated  `applicationContext.xml` to configure constructor injection for `BookService`.

2.    Then I had to  ensure that the `BookService` class has a setter method for `BookRepository` and configure it in `applicationContext.xml`.

2.	Then I had Run the `LibraryManagementApplication` main class to verify both constructor and setter injection.

Exercise 8: Implementing Basic AOP with Spring

Steps:

1. We have to create a package `com.library.aspect` and add a class `LoggingAspect`.

2. Then we will Define advice methods in `LoggingAspect` for logging before and after method execution.

3.  After that we have to Update `applicationContext.xml` to register the aspect and enable AspectJ auto-proxying.

4. Now we will run to test  the `LibraryManagementApplication` main class to verify the AOP functionality.



 Exercise 9: Creating a Spring Boot Application

Steps:

1.	We have to use Spring Initializr to create a new Spring Boot project named `LibraryManagement`.

       2.   We will Include dependencies for Spring Web, Spring Data JPA, and H2 Database.

      3.  Then we will configure database connection properties in `application.properties`.

3.	Here we will create `Book` entity and `BookRepository` interface.

5.  After that we have to create a `BookController` class to handle CRUD operations.

6.  Now , we run the Spring Boot application and test the REST endpoints.

By following these exercises, we can gain hands-on experience in setting up and configuring a Spring application, implementing dependency injection, adding logging with Spring AOP, and creating a Spring Boot application.








WEEK 2 (PL_SQL)
 

This project involves creating and managing a bank database using PL/SQL and  also cover various aspects such as control structures, error handling, stored procedures, functions, triggers, cursors, and packages.
 Exercise 1: Control Structures
1. Discount for Senior Customers:
   1st , The  Loop through customers and apply a 1% discount to loan interest rates for those above 60 years old.
2. VIP Status:
   - Then set IsVIP flag to TRUE for customers with a balance over $10,000.
3. Loan Due Reminders:
   After That , Fetch loans due in the next 30 days and print reminders.

 Exercise 2: Error Handling
1. Safe Fund Transfers:
   Here we will create a procedure to transfer funds between accounts with error handling.
2. Update Employee Salaries:
   Here, Handle errors when updating employee salaries if the employee ID doesn't exist.
3. Add New Customer:
   -The handle exceptions when inserting a new customer if the customer ID already exists.

### Exercise 3: Stored Procedures
1. rocess Monthly Interest
   - 1st we will calculate and update the balance of all savings accounts by applying a 1% interest rate.
2. Employee Bonus Scheme:
   - Then we will update employee salaries by adding a bonus percentage.
3. Fund Transfers Between Accounts:
   - Then we will transfer funds between accounts after checking the source account balance.

 Exercise 4: Functions
1. Calculate Customer Age:
   Then we will function to calculate age from the date of birth.
2. Monthly Loan Installment:
   -Then function to compute the monthly installment for a loan.
3. Check Sufficient Balance:
   The last , Function to check if an account has a sufficient balance for a transaction.

Exercise 5: Triggers
1. 1st we will trigger to update the LastModified column whenever a customer's record is updated.
2. Then we will trigger to log transactions into an AuditLog table.
3. After that we have to trigger to ensure withdrawals do not exceed the balance and deposits are positive.

Exercise 6: Cursors
1.  We will generate Monthly Statements,    PL/SQL block with an explicit cursor to generate statements for all customers.
2. Then the part is to apply Annual Fee, PL/SQL block with an explicit cursor to deduct an annual fee from all accounts.
3.  Here we will  Update Loan Interest Rates , PL/SQL block with an explicit cursor to update loan interest rates based on a new policy.

Exercise 7: Packages
1.  In Customer Management Package , Group procedures for adding, updating customers, and getting customer balance.
2.  Then In Employee Management Package ,Group procedures for hiring, updating employees, and calculating annual salary.
3.  Here In  Account Operations Package ,Group procedures for opening, closing accounts, and getting total balance across all account
The database schema includes tables for Customers, Accounts, Transactions, Loans, and Employees. Sample data is provided for testing the PL/SQL blocks.

How to Use
1. Create Tables:  To Run the provided schema to create the necessary tables,  2. Insert Sample Data: To use the sample data scripts to populate the tables. 3. Execute PL/SQL Blocks: To write and execute the PL/SQL blocks for each scenario .  4.Verify Results: For  checking the results in the database tables to ensure correctness.

This project helps in understanding and implementing various PL/SQL features to manage a bank's database effectively.


