# Ransomeware

- A type of malware that threatens to publish the victim's data or block access unless the ransom is paid. 

  - **Crypto malware** is used to block access 

 

- To counter ransomware, make sure you backup your information. It does take time for you to reset which can cost the company money.



  - **Example** - Cerber is a RaaS platform that appeared in 2016. Cerber took advantage of a Microsoft vulnerability to infect networks. It used AES-256 algorithm to infect backups and personal data. Darkside is also another Ransomeware that has appeared in 2020. 

 



# Trojans 

- The origin of the name Trojan comes from the Greeks and how they captured Troy by hiding in a big wooden horse.



- The software looks completely normal, the goal is to trick the user into running the software such as a spreadsheet or a game but it actually is a virus hence the name Trojan. 

  - The virus is usually hidden from your antivirus and shuts it off in some situations.



- The virus can install a **backdoor** which allows the attacker to gain access into the system again. 



# Remote Acess Trojans (RAT) 

- With a Trojan is installed, a remote administration tool is given to the attacker. 

  - Keylogging, screen recording, copy files, embed more malware can be done through this remote administration tool.



- **Example** - Darknet, a remote access trojan (RAT) developed by Jean-Pierre Lesuer that allowed a user to control a system with a graphical user interface. Tracks users by taking screen captures, keylogging, or password stealing. 



![image](https://user-images.githubusercontent.com/81980702/120059197-87325100-c015-11eb-936f-224875427f3c.png)

> Image of SubSeVen, A RAT interface, 



# Potentially unwanted programs (PUPs) 

- PUPs are unwanted programs installed from another installer in most cases

  - Most anti-virus can identify PUPs

  

- **Examples** - Software backups, toolbar applications, and many more unwanted programs.



# Worms

- A type of malware that replicates in system memory and can spread over network connection rather than infecting files. 

  - A virus is executed only when a user performs an action such as downloading and running an infected executable process.



- The Code-Red worm was infected early versions of Microsoft IIS web server due to **Buffer Overflow Vulnerability**.



- The primary effect of a worm is to consume network bandwidth as the worm replicates. 

  - The worm can also crash an operating system or server applications ( **DoS**).

  - Worms usually have a payload also. 



- **Example** - The Wannacry worm happened in 2017, it installed crypto malware on computers which were then held for ransom. The worm was able to spread to multiple computers. To spread, there was no human intervention involved 



# Fileless virus

- Fileless malware does not write its code to a disk.

 - Uses memory resident to techniques to run its own processes. 



- Fileless malware uses lightweight **Shellcode** to achieve a backdoor on the host.

  - This allows low detection by scanners. 

  - Uses Windows Management Instrumentation ( WMI ) to execute payloads.



- **Example** - the user clicks on a malicious website link. Website exploits a Flash/Java/Windows vulnerability. Launches PowerShell and downloads payload. Runs PowerShell scripts and executes in memory. Adds an auto-start to registry.



# Command and Control

- In a botnet, there is a command and control center that tells the bots what to do.

  - It is the headquarters for the bots. They report to this center.



- **Example** - A computer gets compromised and becomes the control center. That computer then starts recruiting bots.



# Bots 

- The bots are recruited by some sort of malware.

  - Bots are usually installed by a trojan horse. 



- The bots work together and waits for commands from the **command-and-control center**. 



- The groups work together in a botnet and can cause DDoS attacks, relay spam, and another type of computing task 

  - Botnets are for sale



- **Example** - This [website](https://map.lookingglasscyber.com/) shows what botnets are active and possible attacks. 



# Logic Bomb 

- A malicious program or script that is set to run under particular circumstances or in response to a defined event

  -	The logic bomb can be left by someone that had relations with the company or a grudge. 



- The logic bomb can follow time or date or is a user event

  - Logic bombs are hard to trace, there is no digital signature 



- **Example** - In 2013 in South Korea, an email sent to employees had a trojan horse virus attached to it. A day later, the logic bomb went off. Storage and master boot records were deleted off devices showing error “Please install operating system”. 



# Spyware  

- Software that records information about a PC and its users. 

  - Often installed without the user's consent

  - Often a trojan horse 

  - Some spyware has keyloggers 



- **Example** A **keylogger** is spyware that actively attempts to steal confidential information by recording keystrokes. 

- **Example 2** **Adware** is a **PUP** that configures browser reconfigurations such as tracking cookies. Can be installed as a program or as a browser extension.



# Roolkit  

- In windows, malware can only be manually installed with local administrator privileges. 

  - They have to accept the UAC prompt.

  - Viruses like a Trojan cant hide very well but can use common names to look like it is a normal program running.



- Malware running with admin privileges is called a **Roolkit**.

  - The term comes from Unix/Linux where any process running as root has unrestricted access to everything.



-  Modifies core system files in the kernel of a system

    - Becomes invisible to traditional malware detection



- **Example** - Zues/zbot malware was famous for cleaning out bank accounts. The Zbot combines with Necurs Rootkit which makes it impossible to delete zbot. 

- ** Example 2** - US intelligence agencies have deveoped [DarmMatter and QuarkMatter](https://www.pcworld.com/article/3179348/after-cia-leak-intel-security-releases-detection-tool-for-efi-rootkits.html) EFI rootkits.



# Spraying Attack 

- The cybercriminal tries to log in with an incorrect password till they get locked out

  - The attacker uses common passwords 

 



- If the common passwords do not work, they will move on to the next account after it is locked 



- **Example** - An attacker tries 3 common passwords on an account and gets locked out. The attacker then moves on to the next computer.



# Dictionary  

- A password attack that compares encrypted passwords against a predetermined list of possible password values.

  - The common passwords are made by humans.



- There are dictionaries online that are common passwords for someone who works at a specific company. The attacker will then use that to target someone from the company they are looking at. 

  - The dictionary password attacks can substitute letters such as “p&ssw0rd” 

  - Takes time, it is not efficient. 



- **Example** - Discovers common passwords and their hash attached to it such as ninja, dragon, football, letmein. 



# Brute force 

- A type of password attack where an attacker uses an application to try every possible alphanumeric combination to crack encrypted passwords.

  - Tries every password combination until the hash is matched 

  -	A strong hashing algorithm slows things down 



- **Example** - The attacker obtains a file and the hashes with the passwords. They will then use brute force against the hash with multiple letter combinations 



- **Online** 

  	- Very slow 

    -	Most accounts will be locked out	



- **Offline** 

    - Obtains a list of users and hashes 

    - Calculates a password hash and compares it to a stored hash

    - Requires a lot of resources 



# Rainbow tables 

- Tool for speeding up attacks against passwords by precomputing possible hashes.

  - Doesn’t contain every hash

  - Contains pre-calculated hashes 



- You will have to have different rainbow tables for different hashing methods. Windows is different from MySQL.

  - Refines the dictionary approach. 



# Malicious universal serial bus (USB) cable 

- Looks like a normal USB cable 

  - Operating system identifies it as an HID or a human interface Device, A keyboard doesn’t need extra rights or permissions. 

  - Plugin USB cables that only you trust. 



# Malicious flash drive

- A free USB flash drive can a virus on it. It is a bad idea to plug on a flash drive when you do not know what is on it.

  -  An older operating system would automatically run files 



-	Additional electronics inside an infected flash drive can make the computer automatically run a program. 



- **Example**- Attackers can load malware in documents. Can be configured as a boot device. Acts as an ethernet adapter



# Skimming 

- Duplicating a smart card by reading the confidential data stolen

  - Stealing credit card information, usually during a normal transaction 

  - Copies data from a magnetic strip, card number, expiration date, and card holder’s name



- **Example** -ATM skimming that includes a small camera to watch for pins or puts a fake card reader that looks like it is a part of the device when it is actually there just to steal information.



# Card Cloning 

- Duplicates a smart card by physically cloning the crd

  - Usually gets the credit card details from a skimmer 



-	Creates a duplicate of a card that only has a strip, the chip cannot be replicated. 

  - Gift cards are common with card cloning. 



# Adversarial Artificial Intelligence (AI)

- Using AI to identify vulnerabilities and attack vectors to circumvent security systems.

 	- Requires a lot of data training 

	 - Recognizes pattern with the data that is collected 



- **Example** - Used to stop spam, recommend products to an online retailer, prevent car accidents. 



# Supply chain attacks 

- Attackers can infect any step along the way. People trust their suppliers.

  - The supply chain consists of raw materials, manufactures, distributions, and customers





-	One exploit through a third party can give access to the whole supply chain.



- **Example** - 40 million credit card numbers were stolen from a supply chain. It started with an HVAC accompany. The attackers then got into Targets network



# Cloud-based vs. on-premises attacks

- Attacks can happen in two places, on-premises or on the cloud



- Cloud base security

  -  everything is centralized with no cost 



- On-premise security

  -  puts a burden on the client with data center security and infrastructure cost.

  -  allows people in the company to change security while the cloud is upheld with a third party. 



# Cryptographic attacks

- Data is encrypted and the bad guy doesn’t have the key to the encrypted data 

  - Attackers spend a lot of time trying to decrypt 



- Use of weak cipher suites and implementations can represent a critical vulnerability for an organization. 



# Birthday attack 

- A type of attack that exploits weaknesses in the mathematical algorithms used to encrypt weak passwords. It has to have the same inputs with the same encrypted outputs.

  - **Origin** - There 23 students in a classroom. What are the chances of them having the same birthday? It is %50. For 30 it is %70. 



# Collisions 

- Hashes are supposed to be unique; different input data shouldn’t create the same hash 

  - When the same there is the same hash for a different output, It causes the collision



- **Example** Message-Digest Algorithm 5 had collisions



# Downgrade attack

- A cryptographic attack where the attacker exploits the need for backward compatibility.

  - Forces a computer system to abandon the use of encrypted messages in favor of plaintext messages.



- **Example** in 2014, a TLS vulnerability POODLE, forced the encryption to SSL3.0 which has vulnerabilities. 
