Lee H. Sarduy
ASP.NET
Class Discussion 4

1.What is scaffolding? 
-When you use a template to automate code generation. Think of the scaffolding of a building during construction.

2.What is a navigational property? 
-What is a foreign key property? A navigational property can be used to navigate to the object using the dot operator. A foreign key property is a property that allows an object to be referenced from multiple database tables.

3.What is a virtual property? 
-They give Entity Framework a hook into your plain C# classes and enable features such as an efficient change-tracking mechanism.

4.Explain eagar loading. Explain lazy loading. What is the difference between the two? 
-Eager loading is the process whereby a query for one type of entity also loads related entities as part of the query. Eager loading is achieved by use of the Include method. Lazy loading is a design pattern commonly used in computer programming to defer initialization of an object until the point at which it is needed.

5.What is meant by seeding a database? Explain. 
-Let you to create some initial data for the application.

6.What is meant by the happy path? What is meant by the sad path? Give examples of each that are not in the book. 
-It is the code you execute when the model is in a valid state and you can save the object in the database.

8.What is implicit model binding? Explain. 
-Model binding implicitly goes to work when there is an action parameter through which bind attribute can be used to restrict the binding behavior.

9.What is explicit model binding? Explain. 
-Getdate() returns the current date and time, which is perfect for this example. If you want to just return the date, you can cast the getdate() return as date like this, select cast(getdate() as date);.