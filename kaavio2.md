```mermaid
    sequenceDiagram
      participant browser
      participant server

      browser->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
      activate server
      server--> browser: 201 created statuskoodi
      deactivate server

      Note right of browser: Tässä sivulla ei tapahtu muita HTTP pyyntöjä ja selain pysyy samalla sivulla
```

