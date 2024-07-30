# RollingKeyAuthentication
In this project, I have Implemented a Rolling Key Mechanism in Java (Using Socket Programming) for Client Authentication in Server-Client model


## How Algorithm Works: 
1. Generates a list of random numbers using a "linear congruential algorithm" with a pre-defined seed value.
2. The index value of the random number to be used is stored on both sides.
3. The Random number is selected based on the index and both sides compute the Hash value using "SHA 256".
4. Server and Client Sockets are set up.
5. The client sends the Hash to the Server.
6. The Server verifies the Hash and sends the "AUTH_DONE" Message to the Client, Both the Server and Client increment the index value by one.

   Error Handling:
   The Client checks if three consecutive keys are mismatched then It generates a new random index value and sends it to the Server. 


### How to Run
1. Run "Server.java"
2. and then run "Client.java"

### Screenshots 
![image](https://github.com/azimbaldiwala/RollingKeyAuthentication-/assets/83002384/7b5d31e4-d527-4ff9-9d71-343f6b21bd76)

