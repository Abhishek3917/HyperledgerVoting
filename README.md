# HyperledgerVoting

This repository contains the chaincode for managing election candidates using Hyperledger Fabric. The chaincode provides functionality to add, update, delete, and query candidates and their votes.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Chaincode Functions](#chaincode-functions)
  - [InitLedger](#initledger)
  - [QueryCandidateVotes](#querycandidatevotes)
  - [GetAllCandidates](#getallcandidates)
  - [AddCandidate](#addcandidate)
  - [UpdateCandidate](#updatecandidate)
  - [DeleteCandidate](#deletecandidate)
- [Running the Chaincode](#running-the-chaincode)
- [License](#license)

## Prerequisites

Before you can deploy this chaincode, you need to have the following prerequisites installed:

1. Install Docker, Docker Compose, jq, Git, and Go (Golang).
    ```bash
    sudo pacman -S jq git docker docker-compose go
    ```
2. Start Docker and enable it to run at startup:
   ```bash
   sudo systemctl start docker
   sudo systemctl enable docker
    ```
3. Add your user to the Docker group:
    ```bash
    sudo usermod -aG docker username
    ```
4. Reboot your device to apply the changes.
5. Install Hyperledger Fabric binaries, Docker images, and samples.
[Hyperledger Fabric v2.x](https://hyperledger-fabric.readthedocs.io/en/release-2.5/install.html)
## Setup

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Abhishek3917/HyperledgerVoting.git
    