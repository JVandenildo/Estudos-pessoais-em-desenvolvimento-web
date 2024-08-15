# Backend VS Frontend

The front-end is the set of parts that the user interacts with and sees. Various tools and frameworks can be used to make a web page, but at its core, front-end is made up of JavaScript, CSS, and HTML, as well as other static assets, such as videos or images.
Frontend development may be referred to as client-side development. A way of seeing it is the "client" being a human visitor or someone using a web page, however, when saying "client" from a web development perspective, a non-human requester is what this is being referred to. A browser is an example of client, in others circumstances a mobile device is.

## Table of contents

1. [The web server](#the-web-server);
2. [Storing data](#storing-data);
3. [Authorization and authentication](#authorization-and-authentication);
4. [Multiple backend technologies](#multiple-backend-technologies);
5. [References](#references).

## The web server

A web server is a process running on a computer that listens for requests for information over the internet and sends back responses. Each time a user navigates to a website in the browser, the browser makes a request to the web server of that website. Every website has at least one web server. A large company, such as Facebook, has several computers around the world running servers listening for requests.  
The specific format of a request (and the resulting response) is called a **protocol**. An example of a protocol is HTTP, which is used to access websites. When a visitor navigates to a site in their browser, an HTTP request is made to the website elements.  
For a simple website, a client makes a single request. The web server receives this request and sends back to the client a response containing everything needed to view the website. This does not mean that the website is not interactive, just like the static assets, the website is static because once these files are received, it does not move or change.  
The back-end of the web application decides which files to send to the end user, it can happen that, in modern applications, different files are sent to different users. This is called dynamic content.

## Storing data

The backend of modern web applications includes some kind of database. There are many types of databases, but we can divide them into two types:

- Relational Database; and
- Non-relational Database (also known and NoSQL database).

Relational databases store information in tables with columns and rows, non-relational databases may use other systems such as key-value pairs or a document storage model.  
SQL (Structured Query Language) is a language for accessing and altering data stored in relational databases.  
In addition to the database itself, the back-end needs a way to programmatically access, alter, and analyze the data stored there.

## Authorization and authentication

Two important concepts for server-side logic are authentication and authorization.  
**Authentication** is the process of validating a user's identity. One technique for authentication is to use _logins_ with _usernames_ and passwords. These credentials need to be stored securely in the backend database and verified upon arrival.  
**Authorization** controls which user has access to which application features and actions. Certain application actions, such as the edit profile page on a social network, are accessible only to that user.

## Multiple backend technologies

Unlike the front-end, which is built in HTML, CSS, and JavaScript, there is a lot of flexibility in what technology can be used to create the back-end of a web application.  
It is possible to build the back-end in technologies such as PHP, Java, JavaScript, Python, among others. Most developers use frameworks for this type of technology. Some examples of frameworks are:

- [Laravel](https://laravel.com/) ([PHP](https://www.php.net/));
- [Express.js](https://expressjs.com/) ([JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) rodando em [ambiente node](https://nodejs.org/));
- [Ruby on Rails](https://rubyonrails.org/) ([Ruby](https://www.ruby-lang.org/));
- [Spring](https://spring.io/) ([Java](https://www.oracle.com/java/));
- [JSF](https://www.oracle.com/java/technologies/javaserverfaces.html) ([Java](https://www.oracle.com/java/));
- [Flask](https://flask.palletsprojects.com/en/3.0.x/) ([Python](https://www.python.org/));
- [Django](https://www.djangoproject.com/) ([Python](https://www.python.org/));
- [ASP.NET](https://dotnet.microsoft.com/pt-br/learn/aspnet/what-is-aspnet) ([C#](https://dotnet.microsoft.com/pt-br/learn/csharp)).

The collection of technologies used to build the front-end and back-end of a web application is referred to as a stack. For example, the MEAN stack is a stack of technologies for building web applications that use **M**ondoDB, **E**xpress.js, **A**ngularJS, and **N**ode.js. MondoDB is used as the database, Node.js with Express.js for the rest of the back-end, and Angular is used as the front-end framework.

## References

1. [Article from codeacademy](https://www.codecademy.com/article/http-requests) about HTTP request;
2. [MDN documentation](https://developer.mozilla.org/en-us/docs/learn/server-side/first_steps/web_frameworks#a_few_good_web_frameworks) about backend frameworks;
3. [en.wikipedia.org/wiki/MEAN\_(solution_stack)](<https://en.wikipedia.org/wiki/MEAN_(solution_stack)>);
4. [en.wikipedia.org/wiki/LAMP\_(software_bundle)](<https://en.wikipedia.org/wiki/LAMP_(software_bundle)>).
