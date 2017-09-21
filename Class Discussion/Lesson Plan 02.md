Course: ISTA-322
Lesson Plan: 02
Lee H. Sarduy
18 September 2017

1. What is a controller? What does it do?
-Controllers within the MVC pattern are responsible for responding to user input, often making changes to the model in response to user input. In this way, controllers in the MVC pattern are concerned with the flow of the application, working with data coming in, and providing data going out to the relevant view.

2. Explain the relationship between URLs and controller methods.
-They both depend on the ASP.NET routing system to decides how URLs map to controllers and actions. They have a direct 1-1 corospondance.

3. What does it mean to say that, The web is stateless?"
-With the Web, the state of the app for the user essentially vanishes and then is restored with every click.

4. Where in the directory structure of an ASP.NET MVC application do controllers live?
-In the Controllers folder/System.Web.Mvc.Controller.

5. What programming constructs do controllers contain?
-The methods

6. Where are action methods? What do they do?
-In the controller class/Return an instance of a class that derives from ActionResult.

7. What are query parameters?
-Query parameters are parameters passed via the URL.

8. How do action methods receive HTTP query parameters?
-They are retrieved from the request's data collection and located on the HTTP header.