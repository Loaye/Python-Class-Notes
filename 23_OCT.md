# 23 OCT 17
## CLASSES
-----------

Ex:

class Circle(object):
    x = 0
    y = 0
    def __init__(self):
        self.x = 5
        self.y = 7



Nothing is private in Python
_x : Dont mess with this property

## TCP/IP
---------------
ipv4
ipv6
## SOCKET
---------------

import socket

s = socket.socket()

socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
socket.socket(address family, socket type, and protocol)

socket.getaddrinfo('127.0.0.1'm 'http')

### BUILDING SERVER && CLIENT
#### SERVER
---------------
import socket
socket.socket(socket.AF_INET, socket.SOCK_STREAM, socket.IPPROTO_TCP)
server.bind(('127.0.0.1', 3455))
server.listen(1)
conn, addr = server.accept()
connection.recv(8) <----- Determines how much is recieved by bits
server.close() <----- Closes server

####CLIENT
---------------
import socket
socket.getaddrinfo('127.0.0.1', 3455)
client = socket.socket(*socket.getaddrinfo('127.0.0.1', 3455)[1][:3])
client.connect(('127.0.0.1', 3455))
client.sendall('This is a message') <----- python2
client.sendall(u'This is a message'.encode('utf8')) <----- python3
client.close <--- Closes














