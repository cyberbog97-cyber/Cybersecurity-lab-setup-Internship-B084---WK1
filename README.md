# Cybersecurity-lab-setup-Internship-B084---WK1
This is my first  project on github for the networkwalks Internship B084 - WK1 program

# Cybersecurity Lab Setup – NetworkWalks Internship B084 - WK1

## About This Project

For this project, I set up a virtual cybersecurity lab using VirtualBox and Kali Linux as part of my NetworkWalks Internship B084 - WK1 program.

Since I’m still learning cybersecurity, I wanted to get more hands-on experience with setting up a lab and understanding how different security tools work.

The plan was to create a separate environment where I can practise things like network scanning, reconnaissance, and vulnerability assessment without interfering with my main system or other networks.

I also configured a private NAT Network so I can add more virtual machines in the future and use them to practise security testing in my own lab.

## Objectives

These are the main things I wanted to achieve with this project:

- Install and configure VirtualBox.
- Set up Kali Linux as a virtual machine.
- Create a private NAT Network for the lab.
- Configure the network connection for Kali Linux.
- Assign a consistent IP address to the Kali Linux VM.
- Check that the network connection and DNS resolution are working.
- Take a snapshot so I can restore the VM if something goes wrong.
- Document the setup process for future reference.
- Prepare the lab for more cybersecurity projects and practical exercises.

##  What I Plan to Use the Lab For

I created this lab as a place where I can practise cybersecurity skills, try out different tools, and learn from hands-on exercises.

Some of the things I plan to practise include:

- reconnaissance
- Port scanning
- Vulnerability assessment
- Packet analysis
- Web security testing
-penetration testing 
- learning how different security tools work

##  Ethical Use

I will use this lab for learning and authorized security testing only. Any testing outside my own lab will only be carried out on systems I own or have permission to test.


# 🪜 Lab Setup Procedure

## Step 1: Install Winrar

The first thing I did was install Winrar. I needed it to extract the Kali Linux virtual machine files because the package can come in a Winrar archive format.

## Step 2: Install VirtualBox

Next, I installed VirtualBox, which I used to run Kali Linux as a virtual machine on my computer.

This allowed me to set up a separate Sandbox environment for my cybersecurity practice without needing another physical computer or compromising my host machine.

## Step 3: Create the NAT Network

After installing VirtualBox, I created a separate NAT Network for the lab.
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eaf4e884-fd38-45b3-bad4-1c7dcca416ee" />

I used the following settings:

- **Network Name:** NatNetwork
- **IPv4 Prefix:** `10.0.0.0/24`
- **DHCP:** Enabled



I chose a NAT Network because it allows virtual machines connected to the same network to communicate with one another and access external networks.

This will also make it easier for me to add other virtual machines later and use them for authorized security-testing exercises.

## Step 4: Import Kali Linux

Once the network was ready, I downloaded Kali Linux from the official Kali Linux website and imported the virtual machine into VirtualBox.

I configured the network adapter with these settings:

- **Adapter:** Adapter 1
- **Attached to:** NAT Network
- **Network:** NatNetwork
- **Adapter Type:** Intel PRO/1000 MT Desktop
- **RAM:** 4096 MB (4GB)
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e14a31f5-e809-430f-bdcb-6a35d8ebf0c8" />



I also configured a shared folder to make it easier to transfer files between my main operating system and the Kali Linux virtual machine.

## Step 5: Configure the Kali Linux Network

After importing Kali Linux, I worked on its network configuration to make sure it could communicate through the lab network.

The example configuration was:

- **IP Address:** `10.0.0.2`
- **Subnet Mask:** `255.255.255.0`
- **Gateway:** `10.0.0.1`
- **DNS Server:** `8.8.8.8`

<img width="1920" height="1080" alt="Screenshot 2026-10-26 021406" src="https://github.com/user-attachments/assets/a262fa9d-b28f-4f71-990e-fccc4496b273" />


Having a consistent IP address makes it easier to identify my Kali machine and use it during future lab exercises.

## Step 6: Create a Clean VM Snapshot

After setting up the virtual machine and its initial configuration, I created a snapshot in VirtualBox.
<img width="1920" height="1080" alt="Screenshot 2026-10-26 021406" src="https://github.com/user-attachments/assets/b835401d-09a8-43d0-a7a9-f2ec52be1e42" />

**Snapshot name:** `snapshot 1

I created this snapshot so I would have a clean starting point to return to if something went wrong during future experiments.

This is useful because cybersecurity practice can involve changing settings, installing tools, and testing different configurations. Having a snapshot makes recovery much easier.

---

# Lab Connectivity Testing
<img width="1265" height="876" alt="Screenshot 2026-10-26 015438" src="https://github.com/user-attachments/assets/6a358e91-187b-4f1c-b601-491420b7ebf2" />


After completing the setup, the next step was to check that the network was working correctly and that Kali Linux could communicate with other systems.



## Final Thoughts

This is one of my first steps toward gaining practical experience in cybersecurity. I know I still have a lot to learn, but projects like this give me the opportunity to practise, understand the basics better, and improve as I continue my journey in cybersecurity.



#AUTHOR 
Olusoji Samuel 
Cybersecurity intern

#Linkedin profile: https://www.linkedin.com/in/olusoji-samuel-7b0699416/
