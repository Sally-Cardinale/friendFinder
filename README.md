# friendFinder

FriendFinder is a compatibility-based "FriendFinder"/dating application. 

This is a full-stack site which takes in results from user surveys, then compares the 
answers with the existing users and displays the best overall match. 

To get started with this application, the user will need to install the following:
- Node.js 
- express
- path
- nodemon (optional)

To get help with this project the user can refer to the documentation in npm.

<h3> User Experience </h3>

When initally visiting the FriendFinder <strong>HOME PAGE</strong> they will see the following:

![friendFinder-home](/images/friendFinder-home.png)

To take the survey and be matched, the user will press the "Survey" button and be taken to the following <strong>Survey Page</strong>:

![friendFinder-survey](/images/friendFinder-survey.png)

Once the user completes the survey the data will be compared to the existing friends in the friends.js file and a modal pop-up will appear displaying the user's "best match".

<h3>HTML Routing</h3>

The htmlRoutes.js file includes a:
- GET Route to the /survey path which will display the survey page, and
- Default, catch-all route that leads to the home.html which displays the home page.

<h3>API Routing</h3>

The apiRoutes.js file includes a:
- GET  route with the url /api/friends which is used to display a JSON of all possible friends, and
- POST routes /api/friends which is used to handle incoming survey results as well as handle the compatibility logic. 

