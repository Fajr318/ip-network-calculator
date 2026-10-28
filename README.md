    # ip-network-calculator
A beginner-friendly IPv4 network calculator built with Python.
IP Network Calculator

A beginner-friendly Python project that calculates IPv4 network information.

Project Overview

This tool takes an IPv4 address and a subnet prefix as input and displays useful network information.

Features

* Calculates the network address.
* Displays the subnet mask.
* Calculates the broadcast address.
* Shows the prefix length.
* Displays the total number of IP addresses.
* Estimates the number of usable host addresses for common IPv4 subnets.
* Handles invalid input with an error message.

Technologies Used

* Python 3
* Python ipaddress standard library

Example

Input

* IP Address: 192.168.1.10
* Prefix: 24

Expected Output

IP Address: 192.168.1.10
Network Address: 192.168.1.0
Subnet Mask: 255.255.255.0
Broadcast Address: 192.168.1.255
Prefix Length: 24
Total Addresses: 256
Usable Hosts: 254

How to Use

1. Run main.py using Python 3.
2. Enter an IPv4 address when prompted.
3. Enter a subnet prefix, such as 24.
4. Review the calculated network information.

Learning Goals

This project helps develop practical skills in Python programming, IPv4 addressing, subnetting, input validation, and basic network calculations.

Author

Fajr318

This project is part of my learning journey in Network and Communications Engineering.