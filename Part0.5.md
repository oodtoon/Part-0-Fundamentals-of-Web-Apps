**SPA load
```mermaid
SPA pageLoad sequenceDiagram

browser
server

browser-->server: GET https://studies.cs.helsinki.fi/exampleapp/spa
activate server
server-->browser: HTML document
deactivate server

browser-->server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
activate server
server-->browser: main.js
deactivate server

browser-->server: GET https://studies.cs.helsinki.fi//exampleapp/data.json
activate server
server-->browser: data.json
deactivate server
```