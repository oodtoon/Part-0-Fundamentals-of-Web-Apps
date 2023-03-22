**SPA newNote
```mermaid
SPA newNote sequenceDiagram

browser
server

browser-->server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server

**the server creates the new note using JavaScript and sends back as JSON string

server-->browser: application/json
deactivate server
```