# Video_Transmission_OpenCV

In this project the video which is recorded through webcam using OpenCV is transmitted from the client to the server with the help of Socket Programming in Python. This can be implemented within the same computer or on a different system. Here Raw sockets are used which allows direct sending and receiving of IP packets mostly used in security-related applications.

On the Server Side steps involved: 

--> Socket Creation
--> Socket Bind
--> Socket Listen
--> Socket Accept
--> Handle Client
--> Close Client

On the Client Side steps involved:

--> Socket Creation
--> Socket Connect
--> Socket Receive
--> Socket Send
--> Close Socket

Steps involved for Data Transmission

Server Side:
* OpenCV gets video frames of webcam
* With pickle serialize the frames to byte data
* Pack each frame data using struct module
* Send data to client and display frame

Client Side:
* Receive packets and append them to data
* Unpack the data using struct module
* Load the frames using pickle
* Display the frame at client side
