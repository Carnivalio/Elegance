### 1. Requirements are: Achievable? Missing? Unclear?

- Achievable [MORE COMMENTS]

### 2. Any problems and/or challenges that you faced in providing your solution? How you overcame these problems.

- [LIST OF PROBLEMS AND SOLUTIONS]
- PPPoE command doesn't work on *Packet Tracer*, so we decided to use GNS3 instead

### 3. Technical requirements are all technically sound?

- The requirements is technical enough to understand, and gave important information as it is, but 

### 4. Suggested technology, protocol or feature meets requirements?

- The suggested technology, protocol or feature actually meets the requirements, yet we think that ScaCon is better to do 

### 5. Topology - Is the infrastructure optimal? Does the given topology make sense?

- The infrastructure is feasible, but it doesn't seems to make any sense to 

### 6. Design principles - Scalability and flexibility for growth? Redundancy? Aggregation?

- The level of scalability and flexibility on the requirements is actually works, but there are some point to note here, 

### 7. Is there a better solution?

- [IS THERE?]

### 8. ScaCon have received the suggestion that they replace EIGRP with multiarea OSPF. Would you recommend this? Do you envision any problems with this?

- Since EIGRP is actually the property of Cisco, and multiarea OSPF is open to all vendors, it's all depends on what ScaCon are planning to use, if the company want to use routers that are not Cisco, or maybe in the future they might change some of the routers and equipments with other vendors than Cisco, it's better to set the routing technology to multiarea OSPF, but the most important thing here is, EIGRP uses a flat network without areas, whereas OSPF does that. EIGRP is not as complex as OSPF to use, but we personally think that EIGRP should not be used over WAN, because large scale EIGRP implementations can often be more complex than similar scale OSPF implementations because areas inherently scale the deployment by pruning the database depending on area configuration. EIGRP requires that to be done manually by using stub routers or summary addresses. This can break the topology because it will actually filter routes from the topology table, whereas OSPF will always see the topology.
