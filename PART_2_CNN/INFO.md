## What is Microservices?

<img width="794" alt="microservices-logical" src="https://user-images.githubusercontent.com/11850213/94359370-71564000-00c4-11eb-8f32-85bcbf600e2c.png">
	Image Source : https://docs.microsoft.com/en-us/azure/architecture/guide/architecture-styles/microservices


### What is microservice Architecture?

1. can be shotened as MSA
2. a varinat of SOA(service oriented architecture)
3. purpose is to decouple and modularise system services
4. follows the unix philosophy

### Advantages of MIcroservices

1. Seperation of system concerns
2. Language and design agnostic (language independent)
3. Isolated and decoupled deployments (little place to live not dependent on each other and can be deployed independently)
4. smaller services can be simpler to understand (eliminates monolothic way)
5. allows for contionous delivery
6. scale horizontally (can scale services independentaly without touching other services)

### Distanvantages

1. More overhead
2. difficult to test
3. more security concerns (can lead to copuling of services)
4. an increase of communication between services can lead to more load time
5. duplication of code dependencies across services

### How microservices are structured
1. typical structure (in general Microservices have 3 layers - 1.Communication Layer,2 Processing Layer,3. Storage Layer)
	-it is not necessary that each layer requires storage layer

	1.Communication Layer
	`	- typically a RESTfil API
		- should follow HTTP response and request protocol
		- makes call to other internal services
		- may allow access to and from external services
		- should be well documented
		- should be consistent
	2. Processing Layer
		-process request
		-generates responses
		-may use other system such as queues and libraries
	3. Storage layer
		-an optional layer
		-if required each service should have its own DB
		-storage can also be file system

3.API Gateway
	-entry point for all API endpoints
	-Orchestrates API requets
	-Optimizes API requests by collapsing request
	-abstracts implementation form the interface


