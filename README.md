# Decent Framework

A wiki repo for Decent Framework, a framework for building secure distributed applications with enclaves.

## Remote Attestation: DecentRA

Enables mutual remote attestation between different enclave components

### Core components

- DecentRA API
	- C++ library for DecentRA
	- Git Repo: [https://github.com/zhenghaven/decent-ra-api](https://github.com/zhenghaven/decent-ra-api)

- DecentRA Server
	- Implementation of DecentRA Server, which is used for generating SA report
	  for local Decent components
	- Git Repo: [https://github.com/zhenghaven/decent-ra-server](https://github.com/zhenghaven/decent-ra-server)

### Sample Applications

- DecentRide
	- Ride-sharing application built based on the micro-services architecture
	  similar to [Uber](https://dzone.com/articles/microservice-architecture-learn-build-and-deploy-a)
	- Git Repo: [https://github.com/zhenghaven/decent-ridesharing](https://github.com/zhenghaven/decent-ridesharing)

- DecentHT
	- Distributed Hash Table (DHT) implemented with DecentRA, where only authorized
	  Decent components can access the data
	- Git Repo: [https://github.com/zhenghaven/DecentDHT](https://github.com/zhenghaven/DecentDHT)

### Formal Proofs and Benchmarks

- DecentRA Verif
	- Formal verification of the DecentRA protocols using
	  [ProVerif](https://prosecco.gforge.inria.fr/personal/bblanche/proverif/)
	- Git Repo: [https://github.com/zhenghaven/DecentRaVerif](https://github.com/zhenghaven/DecentRaVerif)

- DecentTester
	- YCSB benchmarks on DecentHT
	- Git Repo: [https://github.com/zhenghaven/DecentTester](https://github.com/zhenghaven/DecentTester)
