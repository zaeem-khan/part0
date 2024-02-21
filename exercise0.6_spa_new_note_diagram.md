[![](https://mermaid.ink/img/pako:eNq9VE1vwjAM_StRzrSFDk0jB06btsPQJsFpyoS8xECgTbMkhU2I_z6Xol32IXVCyyl5tl-e7cR7riqNXPCArzVahdcGlh5KaRktBz4aZRzYyF58tQvovxoI3DZ4azm5JeNxiwt2ezNjqxhdEFkWYq0NhlSFdIVFMHZj0oXJ8A1KVyA4lwUHLRGoaLYQ8ZO_Adt9QuynewS7m03uma5UXaKNrZfGb4PPI7AEY8kcuqmkALYwBf6XwHVHfWvYQlDeuPi7zHMK1RCBhFa2m9S9pDdrY9NtLiTfbCTvSU5keDzn_XyY9PMkH8wGQ3FxKfJRml-NniQ_9NI0ff5TBx4fpl0ys7ib2yrivPNrpuRKDAGWbTINCVMeKVJTAj9o5z0K8tR3TR953zhJHldYNhysKY2nGkl7ID-oYzV9t4qL6Gvs8do1hTt9ei4WUARCUZtY-Uk7GY4D4vABw7dtqQ?type=png)](https://mermaid.live/edit#pako:eNq9VE1vwjAM_StRzrSFDk0jB06btsPQJsFpyoS8xECgTbMkhU2I_z6Xol32IXVCyyl5tl-e7cR7riqNXPCArzVahdcGlh5KaRktBz4aZRzYyF58tQvovxoI3DZ4azm5JeNxiwt2ezNjqxhdEFkWYq0NhlSFdIVFMHZj0oXJ8A1KVyA4lwUHLRGoaLYQ8ZO_Adt9QuynewS7m03uma5UXaKNrZfGb4PPI7AEY8kcuqmkALYwBf6XwHVHfWvYQlDeuPi7zHMK1RCBhFa2m9S9pDdrY9NtLiTfbCTvSU5keDzn_XyY9PMkH8wGQ3FxKfJRml-NniQ_9NI0ff5TBx4fpl0ys7ib2yrivPNrpuRKDAGWbTINCVMeKVJTAj9o5z0K8tR3TR953zhJHldYNhysKY2nGkl7ID-oYzV9t4qL6Gvs8do1hTt9ei4WUARCUZtY-Uk7GY4D4vABw7dtqQ)

# sequenceDiagram
    participant browser
    participant server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>browser: HTML document
    deactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.css
    activate server
    server-->>browser: css file
    deactivate server
    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/main.js
    activate server
    server-->>browser: javascript file
    deactivate server

    
    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/data.json
    activate server
    server-->>browser: {"content":"kk","date":"2024-02-21T14:36:29.289Z"},...]
    deactivate server
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: {"message":"note created"}
    deactivate server