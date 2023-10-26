# JeffersonCountyLibrary

## Setup
* Fork and Clone this repository
* Run `update-database`

## Exercise (12 points)

Check out a new branch and complete the following tasks **in order**:
* 2 points - There is a bug in our authentication!  Identity looks like it is set up, but we can't register users.  Find and fix this bug! (Hint: this should only take one line of code)
* 2 points - Right now, anyone can 'check out' a book.  Update the application so that only a logged in user can check out a book.
* 4 points - In this application, we have the ability to create new books.  Improve this functionality by:
  * Add a link from the nav-bar to add a book
  * Make sure only Librarians can add a book
* 2 points - Create a descriptive pull request and merge this branch into main
* 2 points - Take a screenshot of a database query result from pgAdmin that clearly shows which users in your database are librarians.  Update this README to include your screenshot below:
  
![DBQuerryForW3Exam](https://github.com/joe10111/Launch_Mod5Week3Assessment/assets/41969516/e65d3d7e-a0bb-4627-94f1-ebc1344768a4)

## Questions (6 points)

Answer the questions below in this README.  Answer these questions as if you are in an interview!
1. What are roles and claims as they relate to Authentication and Authorization?
Roles is a sub-system of Identity FrameWork that allows us to group Users based on their privileges in the application. When I say privileged I mean both their level of access and what they can do. For example, if I have a new user who just signed up and the developer's account that has been present since the application deployment. I don't want these two users to have the same access to the application. The developer's account should have an Admin role in the Database that allows them to view all users, assign claims to certain users, and maybe even view an admin panel of some sort. The new user should never know that any of those functionalities exist in the application, they should only be able to see the base user functionality. 

2. How do cookies play a role in authentication and authorization?
Cookies play a role in authentication and authorization by acting as almost low-level security measures. What I mean by this is that cookies are visible to the user so they are not the safest even if we encrypt the value there is still the ability to change your own cookies' client side. So we can use them for small non-impactful features. For example, we can use cookies to check if a person is logged in before and make sure they are automatically logged in. 

3. If asked to implement Auth in a new .NET application, would you use the Identity framework?
Yes, I would one hundred percent use the Identity framework. After the initial introduction of the framework, I was skeptical, I hadn't worked with Razor pages like this before and the routing seemed almost hidden. But once I got into using the framework and seeing the routes/structure of the pages I had a much greater understanding and appreciation. The identity framework makes authentication and authorization a breeze to handle and makes me feel like I can trust these systems even though I might not see all of what's happening behind the scenes. For example, it took me so long during our project to make a log-in page that was responsive and would handle incorrect attempts without reloading the page. I had to use a combination of JavaScript and C# to get it working on the backend, but with Identity framework it comes with an extensive login and register system that handles everything so smoothly and effortlessly.

## Rubric

This assessment has a total of 18 points.  Earning 12 or higher is a pass!
