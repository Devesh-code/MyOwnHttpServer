## Mini HTTP Server in C++

This project implements a basic HTTP server in C++ that listens for incoming connections on a specified port, accepts requests, and sends a pre-built response message.

### Features

* Listens for connections on a specified port.
* Accepts incoming connections.
* Sends a pre-built HTML response message.

### Requirements

* C++ compiler (e.g., g++)
* Basic understanding of C++ networking concepts (sockets)

### Build Instructions

1. Compile the source files (`http_Server.cpp` and potentially others) using your preferred C++ compiler:

   ```bash
   g++ http_Server.cpp -o http_server
   ```

   Replace `http_Server.cpp` with the actual list of source files if there are more. This will create an executable named `http_server`.

2. (Optional) You can create a Makefile to automate the build process.

### Usage

1. Run the `http_server` executable, specifying the IP address or hostname to listen on and the port number:

   ```bash
   ./http_server 127.0.0.1 8080  # Listen on localhost (127.0.0.1) port 8080
   ```

2. Open a web browser and navigate to the same IP address and port you specified (e.g., `http://localhost:8080`). The browser should display the pre-built HTML content from the server's response.

### Code Structure

* `http_Server.h`: Defines the `TcpServer` class with member functions for server setup, listening, and handling connections.
* `http_Server.cpp` (or multiple source files): Implements the member functions of the `TcpServer` class.

**Note:** This is a basic example. More robust HTTP servers would handle different request types, parse request headers and body, and generate dynamic responses based on the request.
