# Introduction
> Focused on providing a simplistic environment for Students organize links and access them from the web browser itself.
> Some might Prefer Obsidian as well to create dashboards and track all the work, I will be creating that as well.

## TimeTable
> In order to prepare the time table create an html based table or extract it from you university webpage
> Another project to automate the timetable creation is on the way

## Launcher/Local hosting
> You dont need one but if you want to work with a launcher use <mark>pyinstaller</mark> to compile all the files and launch in a sepcified port
> Also make sure to rename the main page, ie Workspace.html to index.html befor launchin it
> This will be extremely useful if I get the chance to implement a backend in the future
```py

import http.server
import socketserver

PORT = 8000
Handler = http.server.SimpleHTTPRequestHandler

with socketserver.TCPServer(("", PORT), Handler) as httpd:
    print(f"Serving at http://localhost:{PORT}")
    httpd.serve_forever()


```