# Simple Web Application
   
## 1. Start the container
  
  Pro-Tip: Python is pre-installed in ubuntu 20, I am using ubuntu focal

    docker run -p 8080:8080 -it ubuntu bash

## 2. Update packages index in ubuntu container

package index update

    apt-get update

## 3. Install PIP3 using apt-get

Install PIP3

    apt-get install python3-pip

## 4. Install flask and flask-mysql

Install

    pip3 install flask
    pip3 install flask-mysql

## 5. Copy file to /opt

    COPY app.py /opt/

## 6. Start Web Server

   cd /opt
   FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=8080 
    
## 7. Validate the app

Open a browser and go to URL

    http://localhost:8080/                           => Welcome
    http://localhost:8080/getcity                    => Mooresville     
