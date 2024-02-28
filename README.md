# Introduction
> Focused on providing a simplistic environment for Students organize links and access them from the web browser itself.
> Some might Prefer Obsidian as well to create dashboards and track all the work, I will be creating that as well.
Note : <mark> Use Workspace Loader </mark> for upto date work and <mark>Index.html</mark>for stable and clean version 

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
    import webbrowser

    # Define port and handler
    PORT = 8000
    Handler = http.server.SimpleHTTPRequestHandler

    # Server handling
    with socketserver.TCPServer(("", PORT), Handler) as httpd:
        print("Serving at port", PORT)
        
        # Open webpage in default web browser
        webbrowser.open(f'http://localhost:{PORT}')
        
        # Temp hosting
        httpd.serve_forever()

```

<!-- Add Workflows later -->
## Commiting 
> Note for now this is only for personal use
> Will create a commit script later
```gitbash
git add . | git commit -m "message" | git push
```


## Project Plan
- [ ] Add a program to document using commits

### index.html
- [x] Add CSS
- [ ] Tasker App
    - [ ] Tasker-index
        - [ ] Add JS 
    - [ ] Integrate Tasker app with main webpage
- [ ] Time Tables
- [ ] Meetings
    - [ ] Link
    - [ ] Add container for CSS
- [ ] Organize Website into individual components

### Styles.css
- [ ] Use grid layout

