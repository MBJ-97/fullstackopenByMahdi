browser -> server : HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa

    note over the browser : 
    it sends a JSON file to server 
    {
        content : "message sent"
        date:'2021-09-05T11:35:32.476Z'
    }

server -> browser : 201 response {message: note created}

    note over browser : 
    the browser then executes the event handler that displays all the notes 