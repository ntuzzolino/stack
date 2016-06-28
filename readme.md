> Good Questions are hard to come by.... and their answers even more so. As your client, I am requesting you to build me an application that will be the next best thing since sliced bread. -Jake Overall instructor at BCW

###Stackunderflow was built and given to us needing the following features to function like Stackoverflow
1. A place for users to post questions.
2. Each question should be able to have its own list of responses and comments. 
3. Each Response can have its own list of comments.
4. Responses can be marked as solutions.
5. Questions, Responses, and comments can be upvoted or downvoted and should be ordered according to the most votes.
6. Questions should also be sortable by date.
7. Questions should be able to have topic tags attached to help with searching.
8. A search bar should be available and will filter the questions based upon the query.
---------------------------------------------------------------------------------------
This was the first team project we were able to work on at BCW.

The app uses Firebase as its database.
Built with Angular.js 1.5.5

This was a great project to work on because it felt like the closest thing to production code we had started on

I was assigned to a group with 2 classmates I am pretty fond of.
---------------------------------------------------------------------------------------------------
We had to use the forked files at our disposal to add, edit, and build out the rest of the functionality for our StackUnderflow and a good starting point was either the dashboard-component.js or the questions-component.js and their respective views.

###Have you ever seen an object or a building that's so symmetrical that it just felt relaxing to look at? 

>The .js files we were given to work with had been written in Angular.js before components were released. The use of directives and $scope was something I wanted to wash my hands of ever since we began working with the understanding of SOLID principles. 

I can't say I'm a fan of diving into code intended for web applications that do not utilize component based architecture. I am very set in the way that code is evolving across most Languages that aren't as heavily typed that we, as junior developers, should aim towards the use of components and an isolated scope.

I had to condition myself to practice SOLID and OOD principles every time I write an Angular application. 

The single responsibility principle in writing javascript would really help me organize my thought processes. I like to set what my teacher calls the "sanity checkers" quite often when  I am debugging code and tasking controllers to a single component. Using breakpoints and the debugger in chrome dev tools helped me in a monumental way when I was just starting out in Javascript.

I have found that my work ethic is phenomenally more productive when I have a strict routine of organizing my thoughts and testing along with reading the documentation in my free time about best practice. 

###So we began
In three days we had come up with some decent code but the project was originally planned to give us about 7 days to finish instead of 3 and following the weekend we began on new projects in the class, ultimately setting Stackunderflow aside.

When we finished the project, I felt that this was definitely the most complex task list or to-do application we had ever worked on.

Our team's version had foregone proper naming conventions in a majority of the files by one(won't say who) person that we had as our git master. The silly naming conventions for the bulk of the application drove me a little crazy, so I the following week I would spend couple days rewriting almost all of the controllers and components and finally  trying to build out the rest of the functionality required for our project to at least be a decent, functioning application and keeping our code anonymous.

I wrote our project to work with an isolated scope and named  the controllers and functions accordingly, as a "sanity check". And I see myself continuing to make this repo better over time just because I felt like I had a good time working on it and I might need to clone some code in the future for member profiles and data caching.

If I had any advice for junior developers, it would be to stay organized, be flexible with learning new languages, and when you are working on your own projects you need to build things that you are ABSOLUTELY ecstatic about and otherwise just write simple applications until you are completely comfortable with the skills you needed to finish them.

##Member Object and Data Service 
Anytime we wanted to access the memberObject from a controller we had to use `$rootScope`.

This was a good introduction to `$firebaseObject` and Angularfire but in every controller, we would have to left-hand assign a variable similar to `vm.member` with `$rootScope.member` it was repetitive, to say the least when navigating and saving information attached to the user object.

###Database Design

In my time spent watching tutorials and reading documentation on back-end services I learned that saving all of the user information on a parent object(USERS) in a database is and forever will be A BAD way to design tables for the reason that in production code with clients, it's one level of potentially hundreds of thousands of people and their personal information stored on a single table in a Database, and if you needed to write a function to grab a group of people on the list you would be handling an insane amount of information to dive in and retrieve that list people. 

There are many to avoid this when you are writing an application and(not to point any fingers) I think it's a valuable thing to teach at a development boot camp. But for the purpose of this project, the way we did it was fine.


###Gaf Tape

At this point in time, I have heard talk of Shadow DOMs and I'm interested in (without sounding too naive) knowing the difference between $rootScope and a Shadow DOM and how they work on a device drive.

###What we accomplished
Storing Questions, author information, date posted and user auth.

A functioning Question Array and Question component for getting, posting, editing, and deleting thanks to Nora.

A great UX designed by Jason except the awesome background visible now, my new favorite AQUAMARINE!!!

And a well thought out DataService written by Nora and me.

A good working relationship between all three of us.

###What I worked on later

User profile customization, Answers and Comments attached to each question, and an Isolated scope in each component.


###What I want to finish

up-voting, searching and filtering for questions and users, user profile page and direct messaging, marking a correct answer, and reputation.
