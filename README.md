# SalaryAPI
API created for studies. It's supposed to manage salaries.


## Building the server using Docker

It is possible to build the server using Docker. To download this tool go to the Docker website (https://docs.docker.com/compose/install/).
You will also need the latest version of python found at https://www.python.org/downloads/
To build and run the server using this tool, just use the commands:


```
git clone https://github.com/viniciusnau/SalaryAPI.git
cd SalaryAPI
docker pull postgres
docker-compose build
docker-compose up

```

docker-compose up (again if the first time didn't work)

The built server will be answering through port 8000. In this case you will be able to access the API through URl: 0.0.0.0:8000/


## TestCases


To run the tests, you will need to uncomment the database settings that are commented on, and comment on the PostgreSQL database settings.

After that, just run the following commands on the project work directory:


```
pip install pipenv
pipenv install && pipenv shell
./manage.py makemigrations
./manage.py migrate
./manage.py test

```


## Read The Docs

[![Run in Postman](https://run.pstmn.io/button.svg)](https://god.postman.co/run-collection/d426d36e12a143f78e58)
