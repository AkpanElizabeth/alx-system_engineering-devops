0x08-networking_basics_2

LOCALHOST

"localhost" refers to the loopback network interface of a device, commonly identified by the IP address 127.0.0.1. It is used to access the network services that are running on the same device or machine.

When you type "localhost" into a web browser or use it as a destination address for network communication, it directs the request to the local machine itself. In other words, it is a way to refer to your own computer or device.

The term "localhost" is often used when developing or testing web applications or network services. For example, if you are running a web server on your computer, you can access it by entering "http://localhost" into your web browser, and the browser will connect to the web server running on your machine.

It is worth noting that each device has its own localhost. Therefore, when you refer to localhost on your computer, you are referring to your computer specifically, and when someone else refers to localhost on their computer, it would be their computer.

In this example we can see that:

before running the script, localhost resolves to 127.0.0.1 and facebook.com resolves to 157.240.11.35
after running the script, localhost resolves to 127.0.0.2 and facebook.com resolves to 8.8.8.8
If you’re running this script on a machine that you’ll continue to use, be sure to revert localhost to 127.0.0.1. Otherwise, a lot of things will stop working!

What is 0.0.0.0

The IP address 0.0.0.0 is a special address used in networking to represent an invalid or unknown target or network. It has different meanings depending on the context in which it is used:

In the context of network configuration: When an application or network service is configured to listen on 0.0.0.0, it means that it will listen on all available network interfaces or addresses on the system. This allows the service to accept connections from any source IP address.

In the context of routing: In routing tables, 0.0.0.0 is often used as the default route or the "default gateway." It indicates that any IP address that is not explicitly defined in the routing table should be sent to the default gateway for further processing.

In the context of network programming: When a client or server program specifies 0.0.0.0 as the IP address to bind to, it means that it will accept connections from any available network interface or address on the system.

In summary, 0.0.0.0 is used as a placeholder or wildcard address to represent various concepts in networking, such as listening on all interfaces, routing to the default gateway, or accepting connections from any source IP address.

What is the hosts file

The "hosts" file is a plain text file that is present on most operating systems, including Windows, macOS, and Linux. It is used to map hostnames to IP addresses before querying a DNS server. The hosts file allows you to override or define custom mappings between domain names and IP addresses on a local machine.

When a device needs to access a website or network resource, it typically relies on DNS (Domain Name System) to translate the domain name (e.g., www.example.com) into an IP address (e.g., 192.168.1.1). However, the hosts file provides a way to bypass the DNS lookup process and directly associate a domain name with an IP address on the local machine.

The hosts file contains lines that associate IP addresses with hostnames. Each line typically follows a specific format, with the IP address followed by one or more hostnames separated by spaces or tabs. Here's an example entry in the hosts file:

Copy code
127.0.0.1       localhost
