Lee H. Sarduy
ASP.NET
Class Discussion 6

1. Why do we want to validate user input on the client? Why do we want to validate user input on the server?
The client validation logic gives users instant feedback on the information they enter into a form, and is an expected feature in today's web applications. Meanwhile, the server validation logic is in place because you should never trust information arriving from the network.

2. In ASP.NET MVC, what data items are the focus of validation?
Model values.

3. Where do data annotations live in the .NET framework?
System.ComponentModel.DataAnnotations in the .NET framework.

4. Can you stack multiple validation attributes with regard to actions? If so, how many can you stack?
Yes, you can stack an unlimited number of validation attributes with regard to actions.

5. Explain the syntax of [remote]. What does it do?
Inside the attribute you can set the name of the action, and the name of the controller the client code should call. For example: [Remote("CheckUserName", "Account")]. The Remote attribute enables you to perform client-side validation with a server callback.

6. What is a server callback?
A server callback is when you send a value to the server, and compare the value against the values in the database.

7. What is a model builder? When does it run?
It takes the request parameters and puts it in the model.

8. What is the model state? When is it created? How is it created? What does it contain?
The primary side effect of model binding is model state (accessible in a Controller-derived object using the ModelState property). Not only does model state contain all the values a user attempted to put into model properties, but model state also contains all the errors associated with each property (and any errors associated with the model object itself). If any errors exist in model state, ModelState.IsValid returns false.

9. What does the controller action method generally do if the model stat is not valid?
Re-renders the same view that posted the model values.

10. What are the two options for custom validation? Explain your answer.
The two options are to either package validation logic into a custom data annotation or package validation logic into a model object itself. Putting validation logic into a custom data annotation means you can easily reuse the logic across multiple models. Of course, you have to write the code inside the attribute to work with different types of models, but when you do, you can place the new annotation anywhere. On the other hand, adding validation logic directly to a model object often means the validation logic itself is easier to write (you only need to worry about the logic working with a single type of object, and thus you can more easily make assumptions about the state or shape of the object). Reusing the logic, however, is more difficult.