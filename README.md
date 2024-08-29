# Decent Framework

A wiki repo for Decent Framework, a framework for building secure distributed applications with enclaves.


## Primary Projects

*(Ordered from most recent to oldest)*


### Publish/Subscribe system (Decentagram)

These are the implementations for the paper [Decentagram: Highly-Available Decentralized Publish/Subscribe Systems](https://doi.org/10.1109/DSN58291.2024.00037)

The paper can also be accessed via [https://dsn2024uq.github.io/Proceedings/pdfs/DSN2024-6rvE3SSpzFYmysif75Dkid/410500a274/410500a274.pdf](https://dsn2024uq.github.io/Proceedings/pdfs/DSN2024-6rvE3SSpzFYmysif75Dkid/410500a274/410500a274.pdf)


- Submitted Artifact
	- This is the artifact package submitted to the DSN 2024 conference
	- This artifact received the ***Distinguished Artifact Award*** from the DSN 2024 conference
	- The formal DOI for this artifact is [https://doi.org/10.5281/zenodo.10224298](https://doi.org/10.5281/zenodo.10224298)
	- Git Repo: [https://github.com/lsd-ucsc/Decentagram](https://github.com/lsd-ucsc/Decentagram)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/lsd-ucsc/Decentagram/blob/main/LICENSE)
	- Below are the major components of the Decentagram implementation
- On-chain Broker
	- The on-chain broker for Decentagram
	- Git Repo: [https://github.com/lsd-ucsc/decent-pubsub-onchain](https://github.com/lsd-ucsc/decent-pubsub-onchain)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/lsd-ucsc/decent-pubsub-onchain/blob/main/LICENSE)
- Off-chain Broker
	- Please refer to the *DecentEthereum* in
	  [Total Eclipse Detection](#total-eclipse-detection) section for more details
- Decent RA on-chain
	- On-chain smart contract for Remote Attestations of secure enclaves
	- Git Repo: [https://github.com/lsd-ucsc/decent-ra-onchain](https://github.com/lsd-ucsc/decent-ra-onchain)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/lsd-ucsc/decent-ra-onchain/blob/main/LICENSE)
- DecentRevoker
	- Automated revocation of Decent components by using Ethereum smart contracts
	- off-chain broker
		- The off-chain broker for DecentRevoker
		- Git Repo: [https://github.com/lsd-ucsc/DecentRevoker](https://github.com/lsd-ucsc/DecentRevoker)
			- Repo visibility: Public
			- Open source: [MIT license](https://github.com/lsd-ucsc/DecentRevoker/blob/main/LICENSE)
	- on-chain smart contract
		- The on-chain smart contract for DecentRevoker
		- Git Repo: [https://github.com/lsd-ucsc/decent-revoker-onchain](https://github.com/lsd-ucsc/decent-revoker-onchain)
			- Repo visibility: Public
			- Open source: [MIT license](https://github.com/lsd-ucsc/decent-revoker-onchain/blob/main/LICENSE)




### Total Eclipse Detection

These are implementations for the paper [Total Eclipse of the Enclave: Detecting Eclipse Attacks from Inside TEEs](https://doi.org/10.1109/ICBC51069.2021.9461081)

- EclipseMonitor
	- Git Repo: [https://github.com/lsd-ucsc/EclipseMonitor](https://github.com/lsd-ucsc/EclipseMonitor)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/lsd-ucsc/EclipseMonitor/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/lsd-ucsc/EclipseMonitor/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- Ethereum Difficulty Monitor Experiment
	- Git Repo: [https://github.com/zhenghaven/DecentDiffMonitorExpr](https://github.com/zhenghaven/DecentDiffMonitorExpr)

- DecentEthereum
	- A Ethereum Light client running inside of enclave
	- It provides block header hash verification service and smart contract
	  event subscription service
	- Git Repo: [https://github.com/lsd-ucsc/DecentEthereum](https://github.com/lsd-ucsc/DecentEthereum)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/lsd-ucsc/DecentEthereum/blob/main/LICENSE)



### Remote Attestation (DecentRA)

Enables mutual remote attestation between different enclave components

These are implementations for the paper [Secure Distributed Applications the Decent Way](https://doi.org/10.1145/3457340.3458304)

- DecentRA API
	- C++ library for DecentRA
	- Git Repo: [https://github.com/zhenghaven/decent-ra-api](https://github.com/zhenghaven/decent-ra-api)

- DecentRA Server
	- Implementation of DecentRA Server, which is used for generating SA report
	  for local Decent components
	- Git Repo: [https://github.com/zhenghaven/decent-ra-server](https://github.com/zhenghaven/decent-ra-server)

- Sample Applications 1: DecentRide
	- Ride-sharing application built based on the micro-services architecture
	  similar to [Uber](https://dzone.com/articles/microservice-architecture-learn-build-and-deploy-a)
	- Git Repo: [https://github.com/zhenghaven/decent-ridesharing](https://github.com/zhenghaven/decent-ridesharing)

- Sample Applications 2: DecentHT
	- Distributed Hash Table (DHT) implemented with DecentRA, where only authorized
	  Decent components can access the data
	- Git Repo: [https://github.com/zhenghaven/DecentDHT](https://github.com/zhenghaven/DecentDHT)

- Formal Proofs: DecentRA Verif
	- Formal verification of the DecentRA protocols using
	  [ProVerif](https://prosecco.gforge.inria.fr/personal/bblanche/proverif/)
	- Git Repo: [https://github.com/zhenghaven/DecentRaVerif](https://github.com/zhenghaven/DecentRaVerif)

- Benchmarks: DecentTester
	- YCSB benchmarks on DecentHT
	- Git Repo: [https://github.com/zhenghaven/DecentTester](https://github.com/zhenghaven/DecentTester)





## Decent Enclave Library

- DecentEnclave
	- This is the new repo replacing the [decent-ra-api](https://github.com/zhenghaven/decent-ra-api)
	  of the DecentRA project
	- All utility and helper classes and functions have been separated out from
	  the `decent-ra-api` and became individual libraries and repos mentioned
	  in this documentation
	- DecentEnclave is now only focusing on the foundational functionalities
	  of the Decent Enclave framework
	- Git Repo: [https://github.com/zhenghaven/DecentEnclave](https://github.com/zhenghaven/DecentEnclave)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/DecentEnclave/blob/main/LICENSE)




## Utility Libraries

- SimpleUtf
	- A simple and lightweight C++ library used to convert characters among UTF-8, UTF-16, and UTF-32
	- Git Repo: [https://github.com/zhenghaven/SimpleUtf](https://github.com/zhenghaven/SimpleUtf)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleUtf/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleUtf/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- SimpleObjects
	- A simple and lightweight C++ library implements dynamic object types
	- Git Repo: [https://github.com/zhenghaven/SimpleObjects](https://github.com/zhenghaven/SimpleObjects)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleObjects/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleObjects/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- SimpleJson
	- A simple and lightweight C++ library parses JSON encoded messages into
	  SimpleObjects, and encodes SimpleObjects into JSON messages
	- Git Repo: [https://github.com/zhenghaven/SimpleJson](https://github.com/zhenghaven/SimpleJson)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleJson/blob/master/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleJson/actions/workflows/unit-tests.yaml/badge.svg?branch=master)

- SimpleRlp & AdvancedRlp
	- A simple and lightweight C++ library parses RLP and AdvancedRLP encoded
	  messages into SimpleObjects, and encodes SimpleObjects into RLP or
	  AdvancedRLP messages
	- Git Repo: [https://github.com/zhenghaven/SimpleRlp](https://github.com/zhenghaven/SimpleRlp)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleRlp/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleRLP/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- SimpleSysIO
	- Provides virtual classes / interfaces for System IO operations, such as
	  read/write files and TCP connections
	- It also provides implementation for SystemIO outside of an enclave
	  environment, by using C standard library and Boost library
	- Git Repo: [https://github.com/zhenghaven/SimpleSysIO](https://github.com/zhenghaven/SimpleSysIO)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleSysIO/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleSysIO/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- mbedTLScpp
	- This library provides many C++ class wrappers for MbedTLS C objects
	- Git Repo: [https://github.com/zhenghaven/mbedTLScpp](https://github.com/zhenghaven/mbedTLScpp)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/mbedTLScpp/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/mbedTLScpp/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- SimpleBoostSelector
	- A set of CMake scripts utilize CMake's FetchContent module to help you
	  to only fetch the Boost sub-libraries that are needed by your project
	- Git Repo: [https://github.com/zhenghaven/SimpleBoostSelector](https://github.com/zhenghaven/SimpleBoostSelector)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleBoostSelector/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/SimpleBoostSelector/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- SimpleCMakeScripts
	- Provides some helper CMake scripts to setup:
		- Unit test code coverage report
		- Decent Enclave CMake targets
	- Git Repo: [https://github.com/zhenghaven/SimpleCMakeScripts](https://github.com/zhenghaven/SimpleCMakeScripts)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/SimpleCMakeScripts/blob/main/LICENSE)



## Forked Libraries

- MbedTLS
	- Git Repo: [https://github.com/zhenghaven/MbedTLS](https://github.com/zhenghaven/MbedTLS)
	- We added additional CMake targets for DecentEnclave related projects


- wasm-micro-runtime
	- Git Repo: [https://github.com/zhenghaven/wasm-micro-runtime](https://github.com/zhenghaven/wasm-micro-runtime)
	- We added additional CMake targets for DecentEnclave related projects


- wabt
	- Git Repo: [https://github.com/zhenghaven/wabt](https://github.com/zhenghaven/wabt)
	- We added additional CMake targets for DecentEnclave related projects


