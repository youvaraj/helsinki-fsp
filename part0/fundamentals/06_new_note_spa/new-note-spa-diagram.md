```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: xhr
    deactivate server

    Note right of browser: The browser renders the notes with newly added note at the bottom of list
```
