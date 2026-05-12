[arpccc (1).py](https://github.com/user-attachments/files/27627168/arpccc.1.py)[arpccccccc (1).py](https://github.com/user-attachments/files/27627101/arpccccccc.1.py)# 2c.SIMULATING ARP /RARP PROTOCOLS
## AIM
To write a python program for simulating ARP protocols using TCP.
## ALGORITHM:
## Client:
1. Start the program
2. Using socket connection is established between client and server.
3. Get the IP address to be converted into MAC address.
4. Send this IP address to server.
5. Server returns the MAC address to client.
## Server:
1. Start the program
2. Accept the socket which is created by the client.
3. Server maintains the table in which IP and corresponding MAC addresses are
stored.
4. Read the IP address which is send by the client.
5. Map the IP address with its MAC address and return the MAC address to client.
P
## PROGRAM - ARP
## CLIENT:
~~~


import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
address={"FC:B3:AA:EE:8A:90":" 169.254.156.178"};
while True:
    ip=c.recv(1024).decode()
    try:
       c.send(address[ip].encode())
    except KeyError:
       c.send("Not Found".encode())


~~~

## SERVER:
~~~
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    ip=input(" Enter LOGIC ADDRESS : ")
    s.send(ip.encode())
    print("MAC ADDRESS",s.recv(1024).decode())


~~~
## OUPUT - ARP
<img width="855" height="196" alt="Screenshot 2026-05-12 135611" src="https://github.com/user-attachments/assets/db5f95e5-2784-4e41-ac62-5900b88e0977" />




## PROGRAM - RARP
## CLIENT:
~~~


import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
address={"FC:B3:AA:EE:8A:90":" 169.254.156.178"};
while True:
    ip=c.recv(1024).decode()
    try:
       c.send(address[ip].encode())
    except KeyError:
       c.send("Not Found".encode())


~~~

## SERVER:
~~~
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    ip=input(" Enter MAC ADDRESS : ")
    s.send(ip.encode())
    print("Logic Address",s.recv(1024).decode())


~~~



## OUPUT -RARP
<img width="856" height="522" alt="Screenshot 2026-05-12 135031" src="https://github.com/user-attachments/assets/85a2f95f-3c20-4d11-a398-f90008ba851a" />




## RESULT
Thus, the python program for simulating ARP protocols using TCP was successfully 
executed.
