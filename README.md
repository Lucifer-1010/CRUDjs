# CRUDjs
## CRUD Operation using NodeJS ExpressJS MySQL

1.Install nodeJs package and Init application

![image](https://user-images.githubusercontent.com/68159253/144979029-c705b560-fb57-4b3c-854a-3dad88ae7e7d.png)

2.Create a directory and init application
Create an applicate folder and init the project using the following command.
```
npm init
```

3.Install required packages using NPM
    -Express: used to create manage routing and process HTTP requests from the end client.
    -body-parser: used to parse incoming request from the end client.
    -mysql: Node JS driver to connect MySQL and perform CRUD operations.
    -ejs: is templating engine and its used to render HTML pages to end client
    -nodemon: Optional package and Installed globally. It helps us to listen for modifications to files and automatically restart the app server.
 
 Run the following command to install the above mention modules as dependencies for our application.
```
 npm install --save express mysql body-parser ejs
 npm install -g nodemon
```

4. Create a Database Connection
Create a new database with the following name node_crud and  If you create it with the same name it’s better.
To create a database in MySQL, execute the following query
```
CREATE DATABASE node_crud;
```
After creating a database, we need to create a table with the following name users. If you create it with the same name it’s better. To create a table in Database, execute the following query:
```
CREATE TABLE `users` (
  `id` int(11) NOT NULL,
  `name` varchar(150) NOT NULL,
  `email` varchar(150) NOT NULL,
  `phone_no` varchar(25) NOT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;


ALTER TABLE `users`
  ADD PRIMARY KEY (`id`);

ALTER TABLE `users`
  MODIFY `id` int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=1;
```

5.Run the Application using the following command.
```
npm start (OR) nodemon app
```

http://localhost:3000/


## Output:

###### Home page:

![image](https://user-images.githubusercontent.com/68159253/144979787-7caef73e-bdc0-4e96-99d1-209676e86e5c.png)

![image](https://user-images.githubusercontent.com/68159253/144979830-7f6f3a3f-9c46-456f-8265-7e21e37578f7.png)

###### Add operation:

![image](https://user-images.githubusercontent.com/68159253/144979870-6a58843f-0fc9-4b12-81b2-d89a486cb27b.png)

###### Read Operation:

![image](https://user-images.githubusercontent.com/68159253/144979897-a4c4fa16-0f74-4e1f-ab10-a31987ff8d12.png)

###### Update Operation:

![image](https://user-images.githubusercontent.com/68159253/144979933-f854946f-1f3d-4949-bf3b-922db90ae36f.png)

###### Delete Operation:

![image](https://user-images.githubusercontent.com/68159253/144979961-7f8d0beb-1324-447f-ba0c-b243eec9eff7.png)

###### Database Creation:

![image](https://user-images.githubusercontent.com/68159253/144979986-a4553ca1-c24e-4100-be60-2c0371e4c3b3.png)

![image](https://user-images.githubusercontent.com/68159253/144980007-4618263b-4bb2-4df0-adab-7d43b4b87bb5.png)








