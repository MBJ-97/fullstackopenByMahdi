browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
server -> browser : sends the HTML file 
browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server -> browser : sends the main.css file
browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa.js
server -> browser : sends the spa.js file

    note over the browser :
    The browser starts to execute the JS code that needs JSON data from server 

browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server -> browser : gives the JSON file 

    note over the browwser : 
    the browser then starts executing the event handler that renders notes to display
