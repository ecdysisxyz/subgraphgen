# UCS SubgraphGen - The Ultimate Tool for Easy Creation and Deployment of Upgradeable Clone Standard Subgraphs

## Overview
UCS SubgraphGen is a specialized tool designed to streamline the process of creating and deploying subgraphs for contracts based on the UCS (Upgradeable Clone Standard, `ERC-7546: Upgradeable Clone`), a flexible and easy-cloneable smart contract design pattern.

## Features
- ***Easy Subgraph Creation & Deployment***: Simplify the creation and deployment process of subgraphs for contracts based on the Upgradeable Clone Standard with minimal configuration.
- ***Easy Subgraph Upgrade***: Simplify the upgrading of subgraphs when updating the UCS Dictionary.

## Usage
- `ucsgraph init`: initialize the project config file
    - network
    - proxy contract address
    - studio or hosted service
    - subgraph name
    - abi
    - start block
    - auth
- `ucsgraph deploy`: generate && upload
    - `ucsgraph generate`: generate the subgraph files
        - subgraph.yaml
        - schema.graphql
        - src/Proxy.ts: AssemblyScript mappings for each proxy contracts
        - abis/interface.json: ABIs generated via the Dictionary Implementation Search
    - `ucsgraph upload`: deploy subgraph to the Graph Network
- `ucsgraph upgrade`: upgrade the subgraph files
    - abis/interface.json

## TBD
- Solidity-based mappings support
