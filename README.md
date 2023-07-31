# Pentets_Robot_App
Adapted from Pentesting Bible Book  (Khawaja, Gus. Kali Linux Penetration Testing Bible. Wiley, 2021.)

How to run the application : 

on windows terminal in the appropriate directory, run the following command: <python3 .\pentest_robot.py>

preparation : 
                update or install python 
                linux    <apt update>
                         <apt intsall python3-pip>

phase 1
########
validate the input : test if network address is valid
download the module <raw.githubsecurcontent.com/python/cpython/3.9/Lib?ipaddress.py> i savded the content in a python file that i named ip_address.py that handle all the function related to ip address. If the address is not valid, the application will tell you.

phase 2
#########
host scanning 
- the function execute_command, allow to handel terminal command.
- the Class HostScan contains the function that will compute the nmap command <nmap -sn YourNetworkAdrres>. 

phase 3
#########
- port and service scanning functions that enter the nmap command <nmap -sV -p22,3389 --open Ipaddress> which display is the ip address has the port 22(ssh) or 3389(rdp) opened.




                