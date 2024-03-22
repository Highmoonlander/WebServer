# Web Server Project

This project consists of three web servers created in Java where a client can connect to the server by requesting a server socket. The server sends a string in the form of bytes to the client, which the client then receives and displays. The project includes the following web servers:

1. **Single-Threaded Web Server:**
   - In the single-threaded web server implementation, the server serves only one client at a time. This means that the server processes client requests sequentially.

2. **Multi-Threaded Web Server:**
   - The multi-threaded web server implementation allows the server to serve multiple clients concurrently. Before implementing thread pooling, the server was able to handle up to 100 clients simultaneously.

3. **Thread-Pooled Web Server:**
   - The third web server is implemented using a thread pool to handle client requests efficiently.
   - After introducing a thread pool in the multi-threaded web server, the server can now efficiently serve up to 1 million clients.
     <pre>can be adjusted in the source code</pre>
   - This thread-pooled web server architecture allows for improved scalability and performance by managing a pool of threads to process incoming client requests.

## How to Run the Servers

1. **Single-Threaded Web Server:**
   - To run the single-threaded web server:
     - Compile and run the `Server.java` file.
     - Compile and run the `Client.java` file.
     - The server will send a string in bytes to the client, which will be displayed by the client.
    
    ![Single-Threaded Web Server](images/single_threaded_server.png)

2. **Multi-Threaded Web Server:**
   - To run the multi-threaded web server:
     - Compile and run the `Server.java` file.
     - Compile and run the `Client.java` file.
     - The server will send a string in bytes to the client, which will be displayed by the client.

    ![Single-Threaded Web Server](images/single_threaded_server.png)
    ![Single-Threaded Web Server](images/single_threaded_client.png)
      
3. **Thread-Pooled Web Server:**
   - To run the thread-pooled web server:
     - Compile and run the `Server.java` file.
     - Connect clients to the server and observe improved scalability and performance compared to the single-threaded and multi-threaded servers.

## Additional Notes
- Make sure to review and understand the source code for all three servers to grasp the implementation details.
- Feel free to customize and extend the functionality of the servers based on your requirements.
