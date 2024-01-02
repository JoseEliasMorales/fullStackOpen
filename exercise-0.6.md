sequenceDiagram
participant browser
participant server

browser ->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
activate server
server -->> browser: [{ "content": "prueba", "date": "2024-01-02" }, ... ]
deactivate server