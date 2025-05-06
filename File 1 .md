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
--32-bit number

--Format: xxx.xxx.xxx.xxx (each xxx is 0-255)

--Example: 192.168.1.1

--Total possible addresses: ~4.3 billion

2. **IPv6 (Internet Protocol Version 6)**
--128-bit number

--Format: xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx:xxxx

--Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334

--Total possible addresses: ~340 undecillion

                             Categories of IP Addresses
1. **Public IP Address**
--Globally unique

--Assigned by Internet Service Provider (ISP)

--Accessible over the internet

--Example: 203.0.113.1

2. **Private IP Address**
---Used within local networks

---Not routable on the internet

**Reserved ranges:**

---10.0.0.0 to 10.255.255.255

---172.16.0.0 to 172.31.255.255

---192.168.0.0 to 192.168.255.255

3. **Static vs Dynamic IP**

Static IP: **Permanently assigned, doesn't change.**

Dynamic IP: **Temporarily assigned, can change.**

                                    Special IP Addresses

-----127.0.0.1: **Localhost** (loopback address)

-----0.0.0.0: All IP addresses on **local machine**

-----255.255.255.255: **Broadcast address**

                                      COMMON USES
---**Network identification**

---**Location tracking**

---**Network security**

---**Routing**

---**Device addressing**

# 3. DOMAIN NAME SYSTEM


# 4. PROXY & REVERSE PROXY


# 5. LATENCY
