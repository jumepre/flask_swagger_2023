# swagger

Swagger and Flask exercises
# Exercise client - Requests python.
On this exercise the only goal is to be a client as developer using python and requests.
Run the following commands inside the exercise folder:

>pip install -r requirements.txt

>python main.py

# Exercise 0 - Flask python. First local webpage

On this exercise the only goal is to create your first local webpage using python and flask.
Run the following commands inside the exercise folder:

>pip install -r requirements.txt

>python main.py

Then open a url on http://localhost:99


# Exercise 1 - Flask python

On this exercise the only goal is to create your first API where you will invoke different services internally

>pip install -r requirements.txt

>python main.py

Then open a url on http://localhost:99/form

Class Exercise:
- Modify /users/<user_id> call to split it according to the methods.
- Call to methods using postman.

>http://localhost:99/form

>http://localhost:99/login

>http://localhost:99/users/Nuria as GET, POST, DELETE and PUT


# Exercise 2 - Flask python into docker

On this exercise the only goal is to create your first API around a docker file

>docker build --tag python-docker .

>docker run -p 5000:5000 python-docker

Then open a url on http://localhost:5000/form

# Exercise 3 - Swagger python

Let's explore swagger together

>docker build -t swagger_server .

>docker run -p 8080:8080 swagger_server

Then open a url on http://localhost:8080/v2/ui/#/store

https://petstore.swagger.io/#/

https://petstore3.swagger.io/

Nota: https://editor.swagger.io/

# Evaluation Exercise - Create your first API using swagger
Imagine that you work into industry compony where there is a robot. 
We have a sensor that is monitoring the temperature of robot via real-time. The measurement is saving into a database.
Info from sensor;
- id del sensor - string
- fechamuestreo - string
- unidad - string
- medicion - number

Our api needs create the next methods;
> /getLastMeassureBySensor/{sensor}:
sensor -> string

When the methods is successful then this should return;
Measure
- code (id del sensor) - string
- fechamuestreo - string
- unidad - string
- medicion - number
- tipo - string

When the method is not successful then  this should return;
404 -> Invalid ID supplied
400 -> Sensor not found

Steps:
- Create your yaml
- Check the format into https://editor.swagger.io/

