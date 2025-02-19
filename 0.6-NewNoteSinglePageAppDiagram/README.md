```mermaid
sequenceDiagram
    participant browser
    participant server
    participant DOM

    browser->> browser:enters note in the input field
    browser->> browser:clicks Save
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server->>browser: Notes Updated
    deactivate server
    browser->>DOM: updates the DOM by adding the new note



```
