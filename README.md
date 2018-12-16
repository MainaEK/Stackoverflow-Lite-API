StackOverflow-API

StackOverflow-lite is a platform where people can ask questions and provide answers.

forthebadge made-with-python GitHub license Build Status Coverage Status
The required API Endpoints that enable one:

    Register a user
    Login a user.
    Fetch all questions.
    Fetch a specific question.
    Post a question
    Delete a question
    Post an answer to a question
    Mark an answer as accepted or update an answer.

The list of the functioning API Endpoints
Method 	EndPoint 	Functionality
POST 	api/v1/auth/signup 	Register a user
POST 	api/v1/auth/login 	Login a user
GET 	/api/v1/questions 	Fetch all questions
GET 	/api/v1/questions/ 	Fetch a specific question
POST 	/api/v1/questions 	Post a question
Delete 	/api/v1/questions/ 	Delete a question
POST 	/api/v1//answers 	Post an answer to a question
PUT 	/api/v1/questions//answers/ 	Mark an answer as accepted or update an answer.
Installation

Make sure you have Python3 installed on your machine

    Clone this repo and Switch to it

$ git clone https://github.com/erick-maina/Stackoverflow-Lite-API.git
$ cd StackOverflow-API

    Install a virtual Environment and activate it

$ python -m venv venv 	
$ source venv/bin/activate

    Install the dependencies using the requirements file

$ pip install -r requirements.txt

    Run the app

$ export FLASK_ENV=development
$ export FLASK_APP=run.py
$ flask run

Testing the endpoints

    Install postman to test the endpoints

    Open postman and navigate to the localhost and add the enpoint route you are testing

http://localhost:5000/api/v1/<endpoint>

Running tests

To Run the tests you have to use the terminal, switch to the project folder and activate the venv.

    To check if all tests pass

$ pytest 

    To check the test Coverage

$ pytest --cov app  

Technologies used

    Python 3.6
    Flask framework
    Unittest for testing

Author: Eric Maina