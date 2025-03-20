# web-server-golang
Build a Web Server using Golang <br>
This is a simple web server built with Go, which serves static HTML files and handles basic form submissions. The server responds to two routes: a form handler and a hello handler.


**Prerequisites** <br>
You need to have Go installed on your system. You can download and install Go from the official website: https://go.dev/doc/install<br>
Steps to run:
<br>
1. Clone this repository to your local machine:<br>
``git clone https://github.com/rautela-abhiishek/web-server-golang.git``
<br>

The server will start on port 8080.<br>

**Accessing the Server**
1. Open your browser and navigate to http://localhost:8080 to view the static index.html page.
2. Access the form handler by going to http://localhost:8080/form. This route accepts POST requests and displays the submitted data.
3. You can also access the hello handler by visiting http://localhost:8080/hello, which will display a "hello!" message.

**Code Explanation** <br>
<br>
The main.go file starts an HTTP server and defines three routes:
<br>
1. **Root (/):** Serves static files from the /static directory (including index.html and form.html).
2. **Form** **Handler(/form)**: A POST route that handles form submissions. It parses the form data and displays the name and address provided by the user.<br>
3. **Hello Handler** (/hello): A simple GET route that responds with a "hello!" message.<br>
4. **Key Handlers:** <br>

(a). **formHandler(w, r)**: Handles form submissions, parses the form data, and prints the user's name and address.<br>
(b). **helloHandler(w, r)**: Responds with a "hello!" message when accessed via a GET request.
