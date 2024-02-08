(2024, January 18)
01:31
Completed Part1, Part 2 and part 3 


Part 1 - Initial Setup:


Downloaded and installed Visual Studio without encountering any errors.
The installation process took some time but was otherwise straightforward.
Successfully created a sample project in Visual Studio.
Verified project functionality by displaying "Hello World" in the browser.


Part 2 - ASP.NET Core MVC Web Application:


Created a new ASP.NET Core MVC web application using .NET 7.
Encountered an error due to a mistake in Program.cs during the initial setup.
Rectified the error in Program.cs, resulting in a successful outcome.
Verified the correction by observing the browser displaying "Hello Shruti, NumTimes is: 3" when accessing the URL "https://localhost:44342/HelloWorld/Welcome?name=Shruti&numtimes=3."


Part 3 - Adding a View:


Extended the project by adding a view in Part 3.
Followed the prescribed steps for view creation without encountering any errors.
Ensured the seamless integration of the view into the project.


Part 4- 


Successfully installed Visual Studio after encountering initial errors.
Reinstalled Visual Studio to resolve installation issues.

Model Creation and NuGet Packages:

Created a Movie model class with Entity Framework Core for database management.
Encountered a problem with missing packages during initial setup but resolved by building the project.
 
Scaffolding and Database Initialization:

Used scaffolding to generate CRUD pages and a database context.
Faced an issue where the generated pages couldn't be used due to a non-existing database.

Migration and Testing:

Applied EF Core Migrations to create the database.
Overcame an error during testing where the Movie App link did not display the expected result.


Part 5-


Could not examine the database, could not find ssox in the view menu even after restarting so i moved to the next steps

completed seeddata file, had 4 error because of mvc instead of MVC, fixed them
After getting so many errors, i decided to uninstall visual studio and installed it again 

(2024,Jnauary 31)


Part 6-


Updated the Movie.cs model to improve the presentation by using Display and DataType attributes for the "Release Date" field.
Explored the generation of Edit, Details, and Delete links in the Index.cshtml file using Core MVC Anchor Tag Helper.
Examined the MoviesController with both HTTP GET and POST Edit methods for fetching and processing movie data.

Implemented security measures like the [Bind] attribute to prevent over-posting and the [ValidateAntiForgeryToken] attribute to protect against forgery in the HTTP POST Edit method.
Explored the generated HTML for the Edit form and understood the role of anti-forgery tokens.

Highlighted the importance of adhering to HTTP best practices, especially avoiding data modification in HTTP GET methods.
Now I am able to make changes in the list of movies, even individually with url like:https://localhost:7251/Movies/Edit/4 to edit the 4th one.



Part 7-


I got error because i made a mistake in the moviecontroller.cs file but then i removed 3 unnecessary lines and i received the desired result

I then edited that file which allowd me to  pass the search title as route data (a URL segment) instead of as a query string value. i saw the results when i added /Movies/Index/ghost to the url
After that, I added the searh filter fo the movies

I added search by genre now I am able to test the app by searching by genre, by movie title, and by both

(2024, February 1)


Part 8-


Added rating property to the movie model
Completed build after that

Updated the view templates to display, create, and edit the new Rating property in the browser view.

(January, February 8)

I Added Rating R for the movie Harry Met Sally and then ran a build in the packager manager console to update the database.
Received no errors so i moved onto the next part


Part 9-


Edited the Title, Rating, Genre, Price for the movies

The ASP.NET Core documentation was clear and well-organized, making it easy to follow along with the steps.
The tutorial emphasized the MVC principles, especially the importance of keeping code DRY (Don't Repeat Yourself), which made the design and implementation more intuitive.
Adding validation rules to the Movie model using DataAnnotations was straightforward. It helped in enforcing rules consistently across the application.

The integration of client-side validation using jQuery was seamless. Seeing validation errors before submitting the form provided a smooth user experience.
The [HttpPost] Create method worked flawlessly, and ModelState.IsValid accurately detected validation errors on the server side, ensuring data integrity.

The automatic rendering of validation error messages in the form without modifying the controller or views showcased the power of MVC and its ability to adapt to changes.
The documentation provided insights into globalizing the app for non-English locales, demonstrating a comprehensive approach to handling various scenarios.

The uniform application of validation rules without scattering logic across different parts of the application showcased the benefits of the DRY principle.
Understanding how to use DataType attributes for formatting hints and DisplayFormat for specifying date formats added an extra layer of customization.

The ability to set breakpoints and debug the application, even when client-side validation was disabled, ensured a robust validation mechanism.
In summary, the experience was smooth, error-free, and highlighted the strength of ASP.NET Core MVC in building a maintainable and robust web application.


Part 10-

Setting up the ASP.NET Core application was straightforward, following the provided code and scaffolding mechanisms.

The MVC structure, including the Movie controller, was well-organized and easy to understand.
The Details method worked seamlessly, displaying movie details based on the provided ID in a GET request.

The application gracefully handled scenarios where the provided movie ID in the Details method was null or did not correspond to an existing movie.

Integrating Entity Framework for data access was smooth, especially with the use of FirstOrDefaultAsync for querying the database.
The implementation showcased a good security practice by checking for null movie instances to prevent potential issues with malicious URLs.

The Delete method, handling HTTP GET requests, efficiently retrieved and displayed the movie intended for deletion.
The DeleteConfirmed method, responsible for handling HTTP POST requests to delete a movie, had a clear and logical structure.
The use of the ActionName("Delete") attribute provided a clean solution for having two methods (GET and POST) with the same parameter signature.

Following the provided guidance for deploying the application to Azure was successful.
Overall, the implementation was successful, and the absence of errors during testing and deployment highlighted the robustness of the ASP.NET Core application.