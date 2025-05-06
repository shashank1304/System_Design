# 1. CLIENT-SERVER ARCHITECTURE
-----**Client-Server** architecture is a **Network Model** where **client devices (like your computer or phone) request services or data from a central server.**
 

                                             Basic Concepts

Client: **A program or device that sends requests to a server.**

Server: **A program or device that listens for requests from clients and responds to them.**

                                                How It Works

-----Client initiates a **request to the server** (e.g., asking for a webpage).

-----**Server processes the request** (e.g., fetches the HTML page).

-----**Server sends a response** back to the client (e.g., the requested webpage).

-----Client **renders or uses the data as needed**.


                                       Types of Client-Server Architecture
✅ **Two-tier Architecture**

Client <---> Server

Example: Web browser directly talking to a database server (not recommended for large systems).

✅ **Three-tier Architecture**

Client <---> Application Server <---> Database Server

Most common: separates logic, presentation, and data.

✅ **N-tier Architecture**

Adds more layers like caching servers, load balancers, etc., for large-scale systems.

# 2. IP ADDRESS
-----An IP address is a **unique numerical identifier.**

-----Assigned to each **device connected to a computer network** that uses the Internet Protocol for communication.

                                              Types of IP Addresses

1. **IPv4 (Internet Protocol Version 4)**

-----32-bit number

-----Format: xxx.xxx.xxx.xxx (each xxx is 0-255)

-----Example: 192.168.1.1

-----Total possible addresses: ~4.3 billion

2. **IPv6 (Internet Protocol Version 6)**

-----128-bit number

-----Format: xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx

-----Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

-----Total possible addresses: ~340 undecillion

                                          Categories of IP Addresses
1. **Public IP Address**

-----Globally unique

-----Assigned by Internet Service Provider (ISP)

-----Accessible over the internet

-----Example: 203.0.113.1

2. **Private IP Address**

-----Used within local networks

-----Not routable on the internet

**Reserved ranges:**

-----10.0.0.0 to 10.255.255.255

-----172.16.0.0 to 172.31.255.255

-----192.168.0.0 to 192.168.255.255

3. **Static vs Dynamic IP**

Static IP: **Permanently assigned, doesn't change.**

Dynamic IP: **Temporarily assigned, can change.**

                                             Special IP Addresses

-----127.0.0.1: **Localhost** (loopback address)

-----0.0.0.0: All IP addresses on **local machine**

-----255.255.255.255: **Broadcast address**

                                                  COMMON USES
-----**Network identification**

-----**Location tracking**

-----**Network security**

-----**Routing**

-----**Device addressing**

# 3. DOMAIN NAME SYSTEM

 It's like the **Internet’s phonebook**. 
 
 It translates **human-readable domain names (like example.com) into IP addresses (like 93.184.216.34)** that computers use to identify each other on the network.


                                                 How DNS Works
**DNS Resolution Process:**

-----1. User types website name (e.g., **www.google.com**)

-----2. Browser checks local DNS cache

-----3. Query goes through multiple DNS servers

-----4. IP address is returned to browser

-----5. Browser connects to the website

                                                     DNS Hierarchy
**1.Root Servers (.)**

 **2.Top-Level Domain (TLD) Servers**
----(.com, .org, .net, .edu)

----**Country codes**: .uk, .in, .jp

**3.Authoritative Name Servers**

-----Specific to domains

-----Hold actual DNS records

                                                  Common DNS Record Types
-----**A Record**: Maps domain to IPv4 address

-----**AAAA Record**: Maps domain to IPv6 address

-----**CNAME**: Creates domain alias

-----**MX**: Mail server records

-----**TXT**: Text information

-----**NS**: Nameserver records


# 4. PROXY & REVERSE PROXY

                                                      Forward Proxy (Regular Proxy)

A forward proxy sits **between clients and the internet**, 

acting on behalf of clients to:

-----**Hide client identities (anonymity).**

-----**Bypass geo-restrictions.**

-----**Cache content.**

-----**Filter content.**


Structure:          **CLIENT -----> PROXY -----> INTERNET**

                                                           Use Cases
-----Corporate networks.

-----School networks.

-----VPN services.

-----Content filtering.

                                                        Reverse Proxy
A reverse proxy sits **between clients and backend servers**, 

acting on behalf of servers to:

-----**Load balancing.**

-----**SSL termination.**

-----**Caching.**

-----**Security (DDoS protection).**

**STRUCTURE:**               **Internet ----> ReverseProxy ----> Servers**

                                                           Use Cases
-----**Content Delivery Networks (CDN)**

-----**API Gateways**

-----**Load Balancers**

-----**Web Application Firewalls**

                                                       Common Proxy Software
-----**Forward Proxy:** Squid, Nginx

-----**Reverse Proxy:** Nginx, HAProxy, Traefik

-----**Both:** Apache with mod_proxy

                                                     Key Benefits
-----**Security:** Acts as a firewall

-----**Performance:** Caching and compression

-----**Load Distribution:** Balance traffic across servers

-----**SSL Termination:** Handle HTTPS encryption/decryption

-----**Monitoring:** Log and analyze traffic


# 5. LATENCY
Latency is the time delay between the cause and effect of some physical change in the system being observed.

                                                    Types of Latency
**1. Network Latency**

-----Time taken **for data to travel from source to destination**

-----Measured in **milliseconds (ms)**

-----**Components:**

------------------**1. Transmission delay**

------------------**2. Propagation delay**

------------------**3. Processing delay**

------------------**4. Queuing delay**

**2. Application Latency**

-----Time taken **for an application to process a request**

**Includes:**

-----------**Database queries**

-----------**API calls**

-----------**Data processing**

-----------**Rendering time**

                                                  Common Sources of Latency
**1.Physical Distance**

-----Geographic separation between client and server

-----Speed of light limitations

**2.Network Infrastructure**

-----Router hops

-----Network congestion

-----Bandwidth limitations

**3.Server Processing**

-----CPU processing time

-----Memory access

-----Disk I/O

**4.Database Operations**

-----Query execution

-----Index lookups

-----Table scans
