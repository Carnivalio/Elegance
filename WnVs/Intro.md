### Introduction

As ScaCon is originally based on CBD of Sydney and they want to open a branch at Parramatta due to the rapid growth of their business. and as per the requirements, our group has designed a proof of concept for this expansion, we also did the 'test run' on the system to see if it's feasible.

The main requirements from ScaCon are:
- Scalable network designed just in case if business will be expanded again due to the growth
- Perfectly connected connectivity between ScaCon main campus (all Sydney locations) and the new branch (Parramatta)
- Secure communication to ScaCon cloud storage (via ISP)

With the provided WAN solution from ScaCon's Internet Service Provider (OpTel), we managed to set the equipments with these steps (by following the given topology diagram):
- First route we take is setting up the ISP router as it's the main gate of every other equipments, here's the steps that we got through for this router:
	- Set the basic configurations (including the IP assignments)
	- Set the loopback connections
	- Set routing system to be used
	- [WILL BE ADDED LATER TONIGHT]
- We set the Syd1 and Syd2 routers respectively with these steps:
	- [WILL BE ADDED LATER TONIGHT]

Note for basic configurations, we followed the requirements from OpTel, which are:
- Give the name of the equipments as shown in the topology
- Disable the DNS lookup
- Disable the HTTP on every intermediary equipments (switches and routers)
- Enable the Secured Shell connection on all intermediary equipments (switches and routers) and used the related equipments' name as the username and **cisco** for the password
- For the console line, we configure the *logging synchronous*
- Set the warning message for the unauthorized access of users who are prohibited using MOTD banner
- For equipments security we apply these settings:
	- Encrypt the plain text password to prevent the sniffing like attack (e.g. MITM)
	- The privileged EXEC mode secret password is assigned as **class**
	- The VTY and console password is assigned as **cisco**
- Set the clock rate for every external WAN serial links to 128000 kbps (for ScaCon testing purpose)
- Configure the IPv4 and IPv6 of the equipments based on calculated Addressing Table
