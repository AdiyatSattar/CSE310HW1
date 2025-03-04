# CSE310HW1

This assignment basic socket programming for TCP connections in Python, creating sockets, binding specific addresses and ports, and sending and receiving HTTP packets.

### Part 1: Web Server
• Any external libraries used: Socket, Threading, Time

The main library used in this assignment was Socket. Socket was used to create the sockets, binding specific addresses and ports, and sending and receiving HTTP packets. Threading was used to allow the Server and Client to run from one Python file. Time was used to give time for the Server function to run, and allow the Client function to start.

• Instructions on how to run your programs.
In order to run webserver.py, first you need to open a command prompt and open the directory where the file is. For example, the file was in a folder on my OneDrive desktop, so the command I used to open the correct directory was "cd OneDrive/Desktop/Sattar-Adiyat-assignment1". After that, I ran python and the web server itself by using the command "python webserver.py". Once the program is running, I went on a Microsoft Edge page and searched up 'http://localhost:5050/HelloWorld.html'. This outputed the HelloWorld.html file in my directory. To test that the program does not work for files not in the directory, I searched up 'http://localhost:5050/Hello.html', and a '404 Not Found' will be outputed.

• Webpages that your code successfully works for: HelloWorld.html
The web server is able to run .html files in the same directory. The .html file in this directory is HelloWorld, which was able to successfully open. If a file is requested that is not in the directory, a '404 Not Found' error message will be presented. 

### Part 2: Proxy Server


