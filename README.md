# Network_lab_assignment
experiment-1
AIM: Router Configuration (Creating Passwords, Configuring Interfaces)

procedures:
Procedure:
1. Open Packet Tracer:
■ Launch Cisco Packet Tracer on your computer.
2. Create a Simple Network:
■ Drag a router and two computers onto the workspace.
■ Connect each computer to the router using straight-through Ethernet
cables.
3. Access Router CLI:
■ Click on the router, go to the CLI tab.
4. Set Up Passwords:
■ Enter global configuration mode: enable, configure terminal.
■ Set the console password: line console 0, password cisco,
login.
■ Set the enable password: enable password cisco.
■ Set the VTY password: line vty 0 4, password cisco, login.
5. Configure Router Interfaces:
■ Go to interface configuration mode for the first interface: interface
gig0/0.
■ Assign an IP address: ip address 192.168.1.1 255.255.255.0.
■ Enable the interface: no shutdown.
■ Repeat for the second interface: interface gig0/1, ip address
192.168.2.1 255.255.255.0, no shutdown.

6. Configure IP Addresses on Computers:
■ Assign IP address 192.168.1.2 and 192.168.2.2 to the first and second
computer, respectively.

7. Test Connectivity:
■ Use the ping command to test connectivity between the computers
through the router.

procedure commands in cli router 
  no
  enable
  conf t
  int fa 0/0
  ip add 192.168.10.1 255.255.255.0 
  no shutdown
  exit
  int fa 0/1
  ip add 192.168.11.1 255.255.255.0 
  no shutdown
  line console 0
  password cisco 
  login
  line vyt 0 4
  password cisco
  login
  exit 
  exit
  save the file 
  close
  again open router cli
  cisco
   enable 
   open pc 0 command prompt
    ping 192.168.1.2


end 

output 
 successfully configured router , password .
