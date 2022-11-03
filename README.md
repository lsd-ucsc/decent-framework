# Decent Framework

A wiki repo for Decent Framework, a framework for building secure distributed applications with enclaves.


## Essential Libraries

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





## Enclave Framework

- DecentEnclave
	- This is the new repo replacing the [decent-ra-api](https://github.com/zhenghaven/decent-ra-api)(also mentioned below)
	- Most of original implementation of `decent-ra-api` has been decomposed
	  and refactored into repos mentioned in this documentation
	- Git Repo: [https://github.com/zhenghaven/DecentEnclave](https://github.com/zhenghaven/DecentEnclave)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/DecentEnclave/blob/main/LICENSE)





## Blockchain Related Libraries

### Total Eclipse Detection

These are implementations for the paper [Total Eclipse of the Enclave: Detecting Eclipse Attacks from Inside TEEs](https://doi.org/10.1109/ICBC51069.2021.9461081)

- EclipseMonitor
	- Git Repo: [https://github.com/zhenghaven/EclipseMonitor](https://github.com/zhenghaven/EclipseMonitor)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/EclipseMonitor/blob/main/LICENSE)
	- Unit Tests Status: ![Unit Tests](https://github.com/zhenghaven/EclipseMonitor/actions/workflows/unit-tests.yaml/badge.svg?branch=main)

- Ethereum Difficulty Monitor Experiment
	- Git Repo: [https://github.com/zhenghaven/DecentDiffMonitorExpr](https://github.com/zhenghaven/DecentDiffMonitorExpr)

### Light Client

- DecentEthereum
	- A Ethereum Light client running inside of enclave
	- It provides block header hash verification service and smart contract
	  event subscription service
	- Git Repo: [https://github.com/zhenghaven/DecentEthereum](https://github.com/zhenghaven/DecentEthereum)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/DecentEthereum/blob/main/LICENSE)

### Revocation: DecentRevoker

Automated revocation of Decent components by using Ethereum smart contracts

- DecentRevoker
	- Git Repo: (work-in-progress)

### WebAssembly

- DecentWasmCounter
	- Instruments WebAssembly code to insert instruction counters needed by
	  DecentSLA project
	- Git Repo: [https://github.com/zhenghaven/DecentWasmCounter](https://github.com/zhenghaven/DecentWasmCounter)
		- Repo visibility: Public
		- Open source: [MIT license](https://github.com/zhenghaven/DecentWasmCounter/blob/main/LICENSE)





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





## Remote Attestation (DecentRA)

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
