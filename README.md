# 2c.SIMULATING ARP /RARP PROTOCOLS
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
<img width="458" height="224" alt="image" src="https://github.com/user-attachments/assets/2334b8ae-ef79-437a-ab3c-5cd333165de8" />
<img width="554" height="194" alt="Screenshot 2026-05-12 131149" src="https://github.com/user-attachments/assets/e1964a0f-086f-4e57-acbe-ce66ad3a3be5" />

## OUPUT - ARP
<img width="911" height="894" alt="Screenshot 2026-05-12 114104" src="https://github.com/user-attachments/assets/0affe7ae-a74e-46f0-8589-48e9c2aae7c9" />

## PROGRAM - RARP
<img width="830" height="813" alt="Screenshot 2026-05-12 115103" src="https://github.com/user-attachments/assets/ce210daf-8f1a-465a-8277-b70c1c1c6749" />
<img width="554" height="194" alt="Screenshot 2026-05-12 131149" src="https://github.com/user-attachments/assets/e1964a0f-086f-4e57-acbe-ce66ad3a3be5" />

## OUPUT -RARP
<img width="917" height="902" alt="Screenshot 2026-05-12 115239" src="https://github.com/user-attachments/assets/62b12633-972a-4e2d-a8a7-23f69ed98f24" />

## RESULT
Thus, the python program for simulating ARP protocols using TCP was successfully 
executed.
