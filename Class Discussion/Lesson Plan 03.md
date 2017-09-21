Course: ISTA-322
Lesson Plan: 03
Lee H. Sarduy
19 September 2017

1. What is a view?
-The UI and part of Three-Tier Architecture./An engine which is the component responsible for processing a view in order to generate a response for the browser./Used to render some part of the model as a user interface.

2. What is the similarity between view names and controller names? What is the diffrence between the two?
-They are a part of the MVC pattern./Views contain the logic required to display elements of the model to the user—and nothing more, where Controllers are the bridge between views and the model

3. Where in the directory structure of an ASP.NET MVC application do views live?
-Views can be found in the Views folder. Each view is further organized into subfolders based on their controller.

4. What is a ViewBag object? What does it do?
-All data is passed from the controllers to the views via a ViewDataDictionary 
(a specialized dictionary class) called ViewData. The ViewBag leverages the dynamic 
keyword to create a dynamic wrapper around ViewData. ViewBag is just syntactic sugar 
that some people prefer over the dictionary syntax. It just looks nicer.

5. What does the at symbol (@) do? Can you excape it? If so, how?
-The magic character that precedes code instructions./Yes, by using // and /* *? comment delimiters

6. What are view conventions and how do they work?
-Reverse of the default settings

7. What is a ActionResult object? How do these objects interact with views?
-An ActionResult object is an instance of the ActionResult class. 
They contain the information that the view converts into HTML to send to the browser.

8. What are strongly typed views?
-A view intended to render a specific domain type, with shortcuts created by MVC.

9. How does Razor combine HTML and C# code?
-Razor allows you to insert C# code into HTML using the @ sign. 
It effectively converts the code to HTML before it is passed to the browser.

10. Where do layouts live in the directory structure of an ASP.NET MVC application?
-In the shared folder of the Views folder.

11. What are the dfferences between a partial view and a \full view?"
-The partial view itself looks much like a normal view, except it doesn't specify a layout; 
if the layout is specified by a _ViewStart.cshtml page (and not directly within the view), the layout is not rendered.