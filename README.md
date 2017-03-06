# nets-tcp-select-echo

This project requires that you construct a select-driven tcp client and server.

Your server should
* be able to accept and respond to multiple conucurrent clients.
* use sockets in non-blocking mode 
* use select() to determine which sockets are ready for reading, writing, or are in error states
* not use threads 
* only send, receive, or accept from a socket ready for that operation
* disconnect any client that has been idle for more than 60 seconds or whose connection has failed
* Your code should be in the select-project subdir and its documentation should include a README.

You are provided demo code for an non-select driven echo server that only accepts one client.

You should indicate how the grader can verify that your program satisfies these requirements.


Some hints:
* State diagrams may be helpful
* You probably want to create specialized clients that trigger error conditions.
