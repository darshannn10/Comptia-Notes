# Rogue access point

- A point that has been installed on the network without authorization, whether with malicious intent or not.

  - It detects rogue WAPs

  - An unauthorized WAP creates a backdoor to attack a network



# Evil twins

- A wireless access point that deceives users into believing that it is a legitimate network access point

  - It is a WAP masquerading as a legitimate one



# Bluejacking 

- Sending of unsolicited messages to another device via Bluetooth 

  - Typical functional distance is about 10 meters 

  - Personal Area Networks (PANs)



# Bluesnarfing 

- A wireless attack where an attacker gains access to unauthorized information on a device using a Bluetooth connection.

  - First major security weakness in Bluetooth

  - Even a PIN can be brute-forced through

  - Older devices that have access to Bluetooth can be vulnerable



# Wireless Disassociation 

- The network keeps on disappearing; you are not able to stop it

  -  Wireless deauthentication; denial of service attack



- **Example** - 802.11 management frames allow you to find access points and manage QoS. 



# Wireless jamming

- Many different types; constant, random bits / constant, legitimate frames

  - Sent at random times and Reactive jamming; When someone tries to communicate

  -  Needs to be somewhere close 



# Radio frequency (RF) jamming 

- Denial of service attack

  - Decreases the signal-to-noises ratio at the receiving device

  - Sometimes it is not intentional but can be intentional



# Radio-frequency identification (RFID)

- They are everywhere; They are used anywhere to track

  - Radar Technology; No battery 

  - RFID attacks can involve data capture, spoof the reader, denial of service, and decrypt communication



# Near field communication (NFC)

- Two-way wireless communication 

  - payment systems 

  - Bootstrap for other wireless; a token 



- **Examples** Remote capture, Frequency jamming, Relay; on path attack 



# Initialization vector

- An input to a cryptographic primitive being used to provide the initial state. 



- Attack on a wireless network that modifies the IV of a encrypted packet. The attacker can learn the plaintext of one packet then compute the RC4 key. 



# MAC address

- The physical address of a network adapter 

  -  48 Bits / 6 bytes long



* **Example** 8c:2d:aa:4b:98:a7 8C:2d:aa = Manufactur model number 4b:98:a7 = Serial number (speicifc to the address)



- Lan switching 

- forward or drop frames; Based on the MAC address 

  - Gather a list of MAC addresses 



- Maintains a loop-free environment ( Using spanning tree protocol ) 



- the sources mac address and destination mac address get sent to the switch 

  - The switch makes a table of MAC addresses which directs traffic 



- MAC flooding 

- A variation of an ARP poisoning attack where a switch's cache table is inundated with frames from random source MAC addresses

  - The mac table is only so big 



- Attackers send info to the mac table and fill it up which turns the switch into a hub. The hub then can capture all networks for a hacker to take advantage of.



![image](https://user-images.githubusercontent.com/81980702/120088435-142ce700-c0b6-11eb-9221-0e2f732195e7.png)

> Picture of ARP flooding



# MAC cloning

- attacker modifies the mac address to match the mac address of the legitimate device

  - Creates a DoS; Disrupt communication to the legit MAC

  - Manipulate through software 



# Address resolution protocol (ARP) poisoning

- ARP stands for Address Resolution Protocol 

- A network-based attack where an attacker with access to target local network segments redirects an IP address to the MAC address of a computer that is not the intended recipient



- on-path attack that can receive data from two different computers



# DNS poisoning (spoofing)

- A network based attack where an attacker exploits the traditionally open nature of a DNS system to redirect a domain name to an IP address of the attackers choosing

 - Modify the information in a DNS server

 - Modify the client host file 

 - Send a fake response to a valid DNS request 



# Domain hijacking

- Gets access to the domain registration and you have control of where the traffic flows 

  - Brute force is used, Social engineering the password gains access to the email address



- **Example** - The domain change in a Brazilian bank left the hacker under control for 6 hours. The bank had 5 million customers and 27 billion in assets. 



# Universal resource locator (URL) redirection

- Unique identifier used to locate a resource on the internet. It is also referred to as a web address

  - Hacker redirects the URL to a malicious website



# Domain reputation

- If a domain or email servers have been hijacked, they are likely used for spam or distributing malware. 

  - The domain could then be put on a block list. 



- concept wherein a domain reputation API or a similar program is able to assess the reputation of a domain or IP address using a set of data resources.

  - It is used to accept and reject connections.



# Distributed denial-of-service (DDoS)

- Packets can be sent causing the network to stop working

  - Force a server to stop working 

  - Takes a design failure or vulnerability 

  - can be caused for a creative advantage 

  - can be used to create a spoofing attack 

  - can be created by accident; loop or even downloading a big file

  - can be caused with botnets 



- Application DoS

  - Makes the application break or work harder by overflowing with packets

  - A zip bomb can be used in an Application Dos and even cloud base services



- **Operational Technology (OT) DoS**

   - the hardware and software for industrial equipment 



- **Example** - Powergrid can stop operate and even traffic lights can turn all green which is hazardous 



# Malicious scripts 

- Automate task and they have alot of speed 



- **Powershell**

    - .ps1 file extension 

    - Extends command line function 

    - Attacks windows OS



- **Python**

    - General-purpose scripting language 

    - Popular in alot of tech and used for cloud orchestration

    - Attacks infrastructure; Routers, switches, and servers



- **Shell script**

    - Automate and extend the command line 

    - Starts with a shebang

    - Attack Linux/unix environments

    - Controls the os on the command line 



- **Macros** 

    - Automate functions inside an application 

    - Attackers create exploits that execute with macros 



- **Visual Basic For Applications**

    - Automates processes in a Windows application 

    - Code can be run through these processes; very vulnerable.
