# SOA-Project

This is an application created for the SOA course.

The application offers the users the possibility to Login and keep track of their ToDos. Each user can add a new ToDo or delete a ToDo element if he/she thinks that it is no longer necessary. After Loging in the users will see a list of ToDo's, if they have some saved. 
There are 2 types of users: admin and normal user. Since the application is a simple one, at this point the admin and the simple user can perform the same actions.

Documentation can be found inside the project in the folder Documentation.


PROJECT STRUCTURE:
AUTH_API folder contains the authentication part. This returns an API Endpoint POST/login after receiving an JSON type object. After checking if the user appears in the DataBase the AUTH_API will return an access token.

FRONTEND folder contains the UI for the application

K8S is used to deploy the Microservices with Kubernetes

LOG MESSAGE PROCESSOR consumer which awaits for new messages and displays them in console.

TODOSE API performs GET for all ToDo’s, POST for creating a new ToDo and Delete for deleting a ToDo

USER API perform GET for all users and also a GET/users/username for displaying a user based on his username


FOR RUNNING THE APPLICATION
docker-compose up —build

Then access http://127.0.0.1:8080 for web UI
