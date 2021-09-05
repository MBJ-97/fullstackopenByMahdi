browser -> server : HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note  
server -> browser : Does a new HTTP GET to notes 

    note over server : 
    the server then adds the POST infos and push them into the data.json file.

browser -> server :  HTTP GET https://studies.cs.helsinki.fi/exampleapp/notes
server -> browser : Returns HTML code 
browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css 
server -> browser : Returns main.css
browser -> server : HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js 
server -> browser : Returns main.js

    note over browser:
    browser starts executing js-code
    that requests JSON data from server 
    end note.

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{ content: "HTML is easy", date: "2019-05-23" }, ...]

    note over browser:
    browser executes the event handler
    that renders notes to display
    end note.