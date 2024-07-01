```mermaid

sequenceDiagram
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    Server-->>Browser: Loads the root HTML
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    Server-->>Browser: Loads the css
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/spa.js
    Server-->>Browser: Loads the javascript
    Browser->>Server: Sends a request through xhttp "GET", "/exampleapp/data.json"
    Server-->>Browser: Parse the returned JSON 

```