# Axios-middle-layer

For future maintenance of the project, it is considered that multiple databases (cloud database, local cache, local database, etc.) may be used. Axios is a promise-based HTTP library. Simply put, it can send get and post requests. I encapsulated the third-party library axios in the project.

Reason: Every time an http request is sent, an Axios instance must be created. I want to simplify this process. (Decoupling)

Realization process: Pack the network data exchange layer in the project. Using object-oriented programming ideas, create a parent class function, abstract the same methods and attributes every time an Axios instance is created.

# How to use 
you will see 3 Parameters: config, success, failure. And "success" and "failure" are functions.

first put the file in your "src" static directory.(if you use Vue cli 3.0)

First, when you use this supreme class, some basical property will be created, you can change it.

Second, import this JS file in you Component.

Then you can creat an object request to callback 2 functions.(success and failure)


# Attention
You should write your own callback functions. In my JS file is empty. you can write it in component or just in this JS file.

There are 3 files.The Third one privide you use it in asynchronous way.（use ES6 promise）
