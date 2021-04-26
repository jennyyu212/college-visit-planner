# Introduction

This was done as a group project for Brown University's Introduction to Software Engineering course. It was implemented with a Java backend, Spark framework, React/JS frontend, and SQLite database.

# College Visit Planner

A web app to help students plan college tours.
It suggests an optimal route to visit a list of user selected colleges by
* dividing the schools into clusters based on their geolocations using hierarchical clustering
* recommending nearby airports 
* Solving the Travelling Salesman Problem using Christofides algorithm to create road trip routes within each cluster

Deployed at [https://collegetripplanner.herokuapp.com/](https://collegetripplanner.herokuapp.com/) 

## How to Build and Run

1. Run in production mode using Docker

Execute the following commands in the project root directory:

* *docker build collegevisitplanner .* to build the docker image

* *docker run -p 4567:4567 collegevisitplanner* to start the containers

Open [http://localhost:4567](http://localhost:4567) to view it in the browser.

_______

2. Run in development mode

* *cd frontend* to enter frontend directory
* *npm install* to install dependencies
* *npm start* to start the frontend 

* *cd ../backend* to enter backend directory
* *mvn clean package* to install dependencies
* *./run --gui* to run backend

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

