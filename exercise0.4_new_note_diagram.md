[![](https://mermaid.ink/img/pako:eNq9lMFuEzEQhl9l5AOnzSbdliL50AtUUNQCYsMFFiHXnjRud21jj5OiKO_ecTflUuUQgbon65_xP9-M194I7Q0KKRL-zug0vrPqJqqhc8BfUJGstkE5guvo1wnj8wCLq6KPkV3a5Oxs1CV8-dzOYUkUkpxOE2VjMdU61Uvsk3V3tl7YKd6rIfSoQpg6XP9ynnC0U5rsShH-rVLEcT3hGrtqEj7Mry7BeJ0HZKS1pSUQ3hMsLPYGgg-5ZxczRqwLmUYrg88qjIFPjACehaeOqqd-LggiGhtRUwJaInz7egnkWeQJJnqUCk4Fb9u2glfwsd0_nPfnB82GodI_DGZvz0X-P4iDso7DB1LyBj6qHl8K8PZAvlu1UklHG-ilMI0ixZjeHQb6Y9PxjXZUDlvITpjM1p2oeMW7H6Vm1pxMZs2kOZofncjjRr6e1advTr93YlvVdf1zT3OiEgNGnp7h12JTkjrBv_pQTKHYx7tOdG7LeSqTb_84LSTFjJXIoRTfvSxCLlSfWOU7RD5ejc8PMy_sjdg-AJ9lkis?type=png)](https://mermaid.live/edit#pako:eNq9lMFuEzEQhl9l5AOnzSbdliL50AtUUNQCYsMFFiHXnjRud21jj5OiKO_ecTflUuUQgbon65_xP9-M194I7Q0KKRL-zug0vrPqJqqhc8BfUJGstkE5guvo1wnj8wCLq6KPkV3a5Oxs1CV8-dzOYUkUkpxOE2VjMdU61Uvsk3V3tl7YKd6rIfSoQpg6XP9ynnC0U5rsShH-rVLEcT3hGrtqEj7Mry7BeJ0HZKS1pSUQ3hMsLPYGgg-5ZxczRqwLmUYrg88qjIFPjACehaeOqqd-LggiGhtRUwJaInz7egnkWeQJJnqUCk4Fb9u2glfwsd0_nPfnB82GodI_DGZvz0X-P4iDso7DB1LyBj6qHl8K8PZAvlu1UklHG-ilMI0ixZjeHQb6Y9PxjXZUDlvITpjM1p2oeMW7H6Vm1pxMZs2kOZofncjjRr6e1advTr93YlvVdf1zT3OiEgNGnp7h12JTkjrBv_pQTKHYx7tOdG7LeSqTb_84LSTFjJXIoRTfvSxCLlSfWOU7RD5ejc8PMy_sjdg-AJ9lkis)


# sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: HTML document with text field populated with input
    deactivate server

    Note over browser,server: It redirects the URL to request the HTML, CSS, & JS

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
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
    server-->>browser: [{"content":"dunki","date":"2024-02-21T14:32:50.676Z"},...]
    deactivate server