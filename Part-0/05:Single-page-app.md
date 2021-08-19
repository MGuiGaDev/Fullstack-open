# Single page app

## Instructions:

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
server-->browser: HTML-code

note over browser:
browser invokes css-code through <link rel="stylesheet" type="text/css" href="/exampleapp/main.css" />
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css

note over browser:
browser invokes css-code through <script type="text/javascript" src="/exampleapp/spa.js"></script>
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa.js
server-->browser: spa.js

note over browser:
browser starts executing js-code
that request JSON data from server:
    xhttp.open("GET", "/exampleapp/data.json", true)
    xhttp.send()
end note

browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/data.json
server-->browser: [{"content":"newski noteski","date":"2021-08-18T11:42:42.813Z"}, ...]

![image](https://user-images.githubusercontent.com/82242888/129970339-9667dec5-f60f-4b7f-9cc4-4bcb0cbbd65f.png)

