-------------------------------<<<Model-View-Controller (MVC) Challenge: Tech Blog>>>-------------------------------
---------------------------------------------------------------------------------------------------------------------    
    Writing about tech can be just as important as making it. Developers spend plenty of time creating new applications and debugging existing codebases, but most developers also spend at least some of their time reading and writing about technical concepts, recent advancements, and new technologies. A simple Google search for any concept covered in this course returns thousands of think pieces and tutorials from developers of all skill levels!

---------------------------------------------------------------------------------------------------------------------
----------------------------------------------------<<<CHALLENGE>>>--------------------------------------------------
 
    Your challenge this week is to build a CMS-style blog site similar to a Wordpress site, where developers can publish their blog posts and comment on other developers’ posts as well. You’ll build this site completely from scratch and deploy it to Heroku. Your app will follow the MVC paradigm in its architectural structure, using Handlebars.js as the templating language, Sequelize as the ORM, and the express-session npm package for authentication.

---------------------------------------------------------------------------------------------------------------------
---------------------------------------------------<<<USER STORY>>>--------------------------------------------------

    AS A developer who writes about tech
    I WANT a CMS-style blog site
    SO THAT I can publish articles, blog posts, and my thoughts and opinions

---------------------------------------------------------------------------------------------------------------------
---------------------------------<<<<<<<<<<<<<<<<ACCEPTANCE CRITERIA>>>>>>>>>>>>>>>----------------------------------
---------------------------------------------------------------------------------------------------------------------
<<<GIVEN a CMS-style blog site:

1. WHEN I visit the site for the first time
     THEN I am presented with the homepage, which includes existing blog posts if any have been posted; navigation links for the homepage and the dashboard; and the option to log in

2. WHEN I click on the homepage option
     THEN I am taken to the homepage

3. WHEN I click on any other links in the navigation
     THEN I am prompted to either sign up or sign in

4. WHEN I choose to sign up
     THEN I am prompted to create a username and password

5. WHEN I click on the sign-up button
     THEN my user credentials are saved and I am logged into the site

6. WHEN I revisit the site at a later time and choose to sign in
     THEN I am prompted to enter my username and password

7. WHEN I am signed in to the site
     THEN I see navigation links for the homepage, the dashboard, and the option to log out

8. WHEN I click on the homepage option in the navigation
     THEN I am taken to the homepage and presented with existing blog posts that include the post title and the date created

9. WHEN I click on an existing blog post
     THEN I am presented with the post title, contents, post creator’s username, and date created for that post and have the option to leave a comment

10. WHEN I enter a comment and click on the submit button while signed in
     THEN the comment is saved and the post is updated to display the comment, the comment creator’s username, and the date created

11. WHEN I click on the dashboard option in the navigation
     THEN I am taken to the dashboard and presented with any blog posts I have already created and the option to add a new blog post

12. WHEN I click on the button to add a new blog post
     THEN I am prompted to enter both a title and contents for my blog post

13. WHEN I click on the button to create a new blog post
     THEN the title and contents of my post are saved and I am taken back to an updated dashboard with my new blog post

14. WHEN I click on one of my existing posts in the dashboard
     THEN I am able to delete or update my post and taken back to an updated dashboard

15. WHEN I click on the logout option in the navigation
     THEN I am signed out of the site

16. WHEN I am idle on the site for more than a set time
     THEN I am able to view comments but I am prompted to log in again before I can add, update, or delete comments
Mock-Up

<The following animation demonstrates the application functionality:
    --> Animation cycles through signing into the app, clicking on buttons, and updating blog posts.
---------------------------------------------------------------------------------------------------------------------
-----------------------------------<<<<<<<<<<<<<<<<GETTING STARTED>>>>>>>>>>>>>>>------------------------------------
---------------------------------------------------------------------------------------------------------------------

1. Your application’s folder structure must follow the Model-View-Controller paradigm. You’ll need to use the express-handlebars (Links to an external site.) package to use Handlebars.js for your Views, use the MySQL2 (Links to an external site.) and Sequelize (Links to an external site.) packages to connect to a MySQL database for your Models, and create an Express.js API for your Controllers.

2. You’ll also need the dotenv package (Links to an external site.) to use environment variables, the bcrypt package (Links to an external site.) to hash passwords, and the express-session (Links to an external site.) and connect-session-sequelize (Links to an external site.) packages to add authentication.

<NOTE
The express-session (Links to an external site.) package stores the session data on the client in a cookie. When you are idle on the site for more than a set time, the cookie will expire and you will be required to log in again to start a new session. This is the default behavior and you do not have to do anything to your application other than implement the npm package.

---------------------------------------------------------------------------------------------------------------------
------------------------------------<<<<<<<<<<<<<<<<GRADING REQS>>>>>>>>>>>>>>>--------------------------------------
---------------------------------------------------------------------------------------------------------------------
<NOTE
1. If a Challenge assignment submission is marked as “0”, it is considered incomplete and will not count towards your graduation requirements. Examples of incomplete submissions include the following:

1. A repository that has no code
2. A repository that includes a unique name but nothing else
3. A repository that includes only a README file but nothing else
4. A repository that only includes starter code

---------------------------------------------------------------------------------------------------------------------
----------------------------<<This Challenge is graded based on the following criteria:>>----------------------------
---------------------------------------------------------------------------------------------------------------------
<Technical Acceptance Criteria: 40%>

1. Satisfies all of the preceding acceptance criteria plus the following:
2. Application’s folder structure follows the Model-View-Controller paradigm.
3. Uses the express-handlebars (Links to an external site.) package to use Handlebars.js for your Views.
4. Application must be deployed to Heroku.

<Deployment: 32%>

1. Application deployed at live URL.
2. Application loads with no errors.
3. Application GitHub URL submitted.
4. GitHub repository contains application code.

<Application Quality: 15%>

1. User experience is intuitive and easy to navigate.
2. User interface style is clean and polished.
3. Application resembles the mock-up functionality provided in the Challenge instructions.

<Repository Quality: 13%>

1. Repository has a unique name.
2. Repository follows best practices for file structure and naming conventions.
3. Repository follows best practices for class/id naming conventions, indentation, quality comments, etc.
4. Repository contains multiple descriptive commit messages.
5. Repository contains a quality README file with description, screenshot, and link to deployed application.

---------------------------------------------------------------------------------------------------------------------
-----------------------------------------<<<<How to Submit the Challenge>>>>-----------------------------------------
---------------------------------------------------------------------------------------------------------------------
1. You are required to submit BOTH of the following for review:
2. The URL of the functional, deployed application.
3. The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

<ADDITIONAL NOTES:
1. You are allowed to miss up to two Challenge assignments and still earn your certificate. If you complete all Challenge assignments, your lowest two grades will be dropped. If you wish to skip this assignment, click Next, and move on to the next Module.
2. Comments are disabled for graded submissions in BootCamp Spot. If you have questions about your feedback, please notify your instructional staff or the Student Success Manager. If you would like to resubmit your work for an improved grade, you can use the Resubmit Assignment button to upload new links. You may resubmit up to three times for a total of four submissions.>