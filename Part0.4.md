**newNote
```mermaid
newNote sequenceDiagram
browser
server

browser-->server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
activate server
server-->browser: redirect new GET to https://studies.cs.helsinki.fi//exampleapp/notes
deactivate server

browser-->server: GET https://studies.cs.helsinki.fi//exampleapp/notes
activate server
server-->browser: HTML document
deactivate server


browser-->server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
activate server
server-->browser: main.css file
deactivate server


browser-->server: GET https://studies.cs.helsinki.fi//exampleapp/main.js
activate server
server-->browser: main.js
deactivate server


browser-->server: GET https://studies.cs.helsinki.fi//exampleapp/data.json
activate server
server-->browser: data.json
deactivate server
```