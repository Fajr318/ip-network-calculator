# ip-network-calculator
A beginner-friendly IPv4 network calculator built with Python.
import ipaddress

ip = input("Enter IP address: ")
prefix = input("Enter subnet prefix (e.g. 24): ")

try:
    network = ipaddress.ip_network(f"{ip}/{prefix}", strict=False)

    print("\n--- Network Information ---")
    print("IP Address:", ip)
    print("Network Address:", network.network_address)
    print("Subnet Mask:", network.netmask)
    print("Broadcast Address:", network.broadcast_address)
    print("Prefix Length:", network.prefixlen)
    print("Total Addresses:", network.num_addresses)

    if network.prefixlen <= 30:
        print("Usable Hosts:", network.num_addresses - 2)
    else:
        print("Usable Hosts:", network.num_addresses)

except ValueError:
    print("Invalid IP address or subnet prefix.")