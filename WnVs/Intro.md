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
	- Set the ISP router so it can support the HDLC and PPP from Syd routers
- We set the Syd1 and Syd2 routers respectively with these steps:
	- Set the basic configurations (including the IP assignments)
	- Connect serial cables to ISP on both routers
	- Connect fast ethernet cable between the routers
	- Set routing system to be used (EIGRP) on both routers
	- Use HSRP to First Hop Redundancy (FHR) on both routers, set Active the Load Balance and Standby between the routers
	- Set up the HDLC between router Syd1 and ISP
	- Set up the PPP technology on ISP and Syd2
	- Set routing system to be used (EIGRP)
- Next is setting the three switches (SwT, SwM, SwB, including PCM and PCS):
	- Set the basic configurations (including the IP assignments on VLANS)
	- Connect fast ethernet cables from SwT to Syd1 and Syd2
	- Connect fast ethernet cables between switches (2 of each), also cable from SwT and SwB
	- Connect PCM with SwM with fast ethernet cable
	- Connect PCS with SwB with fast ethernet cable
	- Set only 3 ports per VLAN per switch to be used
	- Put unassigned ports into the BlackHole VLAN (666), also disable them and then delete the VLAN
	- Assign Management VLAN and Native VLAN on VLAN 150
	- Set the configured VLANs only to be permitted on trunk links
	- Load balance VLANs between all HQ switches by manipulating the Spanning Tree
	- Set the EtherChannel technology between SwM and SwB (using PAgP because it can negotiate between two channels and prevent looping to be happened)
	- Limit the Sales VLAN access, they can only access within same VLAN (Sales)
	- Set Engineering VLAN so it can gain the access permit to reach users on the VLAN and the Internet
	- Set on required equipments so PCM is the only device which can manage all the routers and switches
- Then we set the Syd3 router:
	- Set the basic configurations (including the IP assignments)
	- Connect fast ethernet cable between Syd3 router and SwB
	- Set routing system to be used (EIGRP)
	- Set the router to be able to connect through GRE tunnel with Parra router
- After all of those, we moved to Parramatta branch:
	- Set the basic configurations on all equipments (including the IP assignments)
	- Connect serial cable from Parra router to Syd1
	- Connect fast ethernet cable from Parra router to switch PSW
	- Connect fast ethernet cable from Liv router to switch PSW
	- Connect PCP to Parra router and PCL to Liv router with ethernet cables respectively
	- Set routing system to be used (EIGRP on Parra router and Static routing on Liv router)
	- Set the GRE tunnel connection between router Parra and Syd3 (point-to-point tunnelling)
	- Set the EIGRP routing updates and adjacencies between Parra and main campus through GRE tunnel
	- Set up PPPoE in between Parra router and PSW switch

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
- Swithces specific:
	- Use rapid-PVST+ technology
