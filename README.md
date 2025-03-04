# CSE310Assignment1

This assignment involves basic socket programming for TCP connections in Python, where we create sockets, bind specific addresses and ports, and send and receive HTTP packets.

## Part 1: Web Server

### External Libraries Used
- **Socket**: Used to create the server socket, bind it to a specific address and port, and send and receive HTTP requests and responses.
- **Threading**: Enables concurrent execution, allowing both the server and client to run in the same Python file.
- **Time**: Provides delays to allow the server function to run before the client starts.

### Running the Web Server

To run the **webserver.py** file:
1. Open a command prompt and navigate to the directory containing the file. For example:
cd OneDrive/Desktop/Sattar-Adiyat-assignment1
2. Start the web server by running:
python webserver.py
3. Open your web browser and visit:
http://localhost:5050/HelloWorld.html
This should display the `HelloWorld.html` file in your directory.

4. To test error handling, try accessing a non-existing file:
http://localhost:5050/Hello.html

This will display a `404 Not Found` error.

### Supported Web Pages

- **HelloWorld.html**: Successfully served from the same directory.
- **.jpg files**: Successfully served from the directory.
- **404 Error**: Files not found in the directory will result in a `404 Not Found` error.

## Part 2: Proxy Server

### External Libraries Used
- **Socket**: Used for creating the proxy server socket, binding it to a specific address and port, and handling HTTP requests between clients, websites, and the proxy server.

### Running the Proxy Server

To run the **proxyserver.py** file:
1. Open a command prompt and navigate to the directory containing the file. For example:
cd OneDrive/Desktop/Sattar-Adiyat-assignment1
2. Run the proxy server:
python proxyserver.py
3. The program will prompt you to enter the IP address. Use `127.0.0.1` for the localhost IP.
4. Set up a manual proxy server in your Windows settings:
- Proxy IP: `127.0.0.1`
- Proxy Port: `6060`

5. Once the proxy server is configured, the proxy server will start handling HTTP requests.

### Supported Web Pages

The proxy server successfully handles the following HTTP websites:
- http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file2.html
- http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file3.html
- http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file4.html
- http://gaia.cs.umass.edu/wireshark-labs/HTTP-wireshark-file5.html
- http://www.example.com

**Note**: The proxy server only handles HTTP requests. It does not support HTTPS requests. For example, HTTPS websites like `https://www.google.com` will not work with this proxy server.
