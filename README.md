### Data visualization App
![alt text](https://github.com/ColinRosati1/smart-steel-app/blob/master/smart%20steel%20grab.PNG)

### Overview

Handle Python Backend data in front end. 
Front end visualizes sensor data using Highcharts.

### Task 

Task is to create intuitive page(s) that contain informative visualizations 
of the provided data. Use HTML, JS and CSS to read the JSON and display it in an
organized way. The aim of the page(s) and visualizations should be to explore 
and understand the data for a statistical analysis.



### Context
React, Highcharts, Sass, Jest, Python


### Proposed Solution
I have decided to use react to handle the frontend for its use of states, builds,
project management, testing capabilities. I enjoy the use of state and async states 
in JS suitable for data visualization.

To handle the python flask endpoint I use a fetch call when my SteelApp component first mounts.
Once data response is recieved it is passed through a series of async call to coerse data into JSON,
set data into state and catch errors while trigger an error state as well as call the api function again.

To display the data I have used the suggested Highcharts as it is an elegant solution to style, display 
interactive data. I have modified some of the Highcharts options to suit styling the data.

In the end I have written a few unit tests for the API to make sure it returns data with the corrent amount
of keys needed for all the sensors and data.

### The strengths of this design
clean visualization
quick component rendering
modular components make for readability
clearly defined state handling


### weakness of design
lacks interactivity in data visualization
not responsive
no integration testing
lacks context for sensor data



### TODOS
Write highcharts into its own modular component.
Add responsive styling of app.
Interactive data visualization, zoom in, alternative displays, custom views
Test react DOM compoents
write e2e tests simulating DOM interactions.



### Steps to Run
turn on server  python-server/ python -m main
start react     npm start

app will open on localhost:5000/




