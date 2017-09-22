### 1. Requirements are: Achievable? Missing? Unclear?

- Achievable, [MORE COMMENTS]

### 2. Any problems and/or challenges that you faced in providing your solution? How you overcame these problems.

- Since we're not familiar with the command that would enable the PPPoE on *Packet Tracer*, we realize that it's not (yet) achievable to build the infrastructure on *Packet Tracer*, but the command is available on real equipments, which makes us to be able to simulate the topology on real equipments [EXPAND]
- Unclear port on switch SwB to connect to Syd3 router [EXPAND - DUPLICATE (Explain differently)]

### 3. Technical requirements are all technically sound?

- The requirements is technical enough to understand, and gave important information as it is, but ... 
- Unclear port on switch SwB to connect to Syd3 router [EXPAND - DUPLICATE (Explain differently)]

### 4. Suggested technology, protocol or feature meets requirements?

- The suggested technology, protocol or feature actually meets the requirements, yet we think that ScaCon is better to do ... 

### 5. Topology - Is the infrastructure optimal? Does the given topology make sense?

- The infrastructure is feasible, but it doesn't seems to make any sense to ... 

### 6. Design principles - Scalability and flexibility for growth? Redundancy? Aggregation?

- The level of scalability and flexibility on the requirements is actually works, but there are some point to note here, ... 

### 7. Is there a better solution?

- Use OSPF for whole infrastructure [EXPAND]
- [IS THERE MORE?]

### 8. ScaCon have received the suggestion that they replace EIGRP with multiarea OSPF. Would you recommend this? Do you envision any problems with this?

- Since EIGRP is actually the property of Cisco, and multiarea OSPF is open to all vendors, it's all depends on what ScaCon are planning to use, if the company want to use routers that are not Cisco, or maybe in the future they might change some of the routers and equipments with other vendors than Cisco, it's better to set the routing technology to multiarea OSPF, but the most important thing here is, EIGRP uses a flat network without areas, whereas OSPF does that. EIGRP is not as complex as OSPF to use, but we personally think that EIGRP should not be used over WAN, because large scale EIGRP implementations can often be more complex than similar scale OSPF implementations because areas inherently scale the deployment by pruning the database depending on area configuration. EIGRP requires that to be done manually by using stub routers or summary addresses. This can break the topology because it will actually filter routes from the topology table, whereas OSPF will always see the topology. So, in conclusion, we personally suggest that ScaCon use OSPF because of its ability covering the scalability of the network and also because it's open to any vendors.

## Note

- EIGRP noted capabilities are:
	- **Fast convergence:** a router stores all its neighbors routing tables so that it can quickly adapt to alternate routes.
	- **Variable length subnet mask:** it supports variable length subnet masks permits routes to be automatically summarized on a network.
	- **Support for partial updates:** EIGRP sends partial updates when the metric for a route changes. Propagation of partial updates is automatically bounded so that only those routers that need the information are updated.
	- **Support for multiple network layer protocols:** EIGRP supports AppleTalk which redistributes routes learned from RTMP, IP redistributes routes learned from OSPF and RIP, ISIS, EGP, and BGP, and Novell NetWare implementation redistributes routes learned from Novell RIP or SAP.
- OSPF noted features:
	- **Scalability:** OSPF is specifically designed to operate with larger networks.
	- **Full subnetting support:** OSPF can fully support subnetting
	- **Hello packets:** OSPF uses small hello packets to verify link operation with out transferring large tables
	- **TOS routing:** OSPF can route packets by different criterion based on their type of service field
	- **Tagged routes:** Routes can be tagged with arbitrary values, easing interoperation.
