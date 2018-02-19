# C# Smart Contract Developers Guide

NEO Blockchain Documentation for .NET Developers ([url](https://github.com/mwherman2000/neo-windocs/tree/master/windocs))

## Appendix C - Sample Smart Contracts

### Purpose

TODO

### Goals, Non-Goals and Assumptions

TODO

### Principles

TODO

### Drivers

TODO

## Sample Smart Contracts

### First dApps Competition [DAPPSCOMPETE1]

>A few days ago, the first City of Zion dApps competition submission deadline was reached, and 17 valid projects were submitted. This post provides a brief overview of each project and the integrated components. The projects are presented in alphabetical order. [Chris Hager, Nov 23, 2017]

The following is a list of the links to the smart contracts in each project (some projects have two smart contracts).

1. [Splyse/neo-smart-iot](https://github.com/Splyse/neo-smart-iot/blob/master/neo-pubsub.py) from [https://github.com/Splyse/neo-smart-iot/blob/master/neo-pubsub.py](https://github.com/Splyse/neo-smart-iot/blob/master/neo-pubsub.py)
2. [Splyse/neo-smart-iot](https://github.com/Splyse/neo-smart-iot/blob/master/elcaro-contract.py) from [https://github.com/Splyse/neo-smart-iot/blob/master/elcaro-contract.py](https://github.com/Splyse/neo-smart-iot/blob/master/elcaro-contract.py)
3. [neoauth/smart-contract](https://github.com/neoauth/smart-contract/blob/master/src/NeoAuth.py) from [https://github.com/neoauth/smart-contract/blob/master/src/NeoAuth.py]https://github.com/neoauth/smart-contract/blob/master/src/NeoAuth.py()
4. [BlockSaver/smart-saving-contract](https://github.com/BlockSaver/smart-saving-contract/blob/master/SmartSavingContract/SmartSavingContract.cs) from [https://github.com/BlockSaver/smart-saving-contract/blob/master/SmartSavingContract/SmartSavingContract.cs](https://github.com/BlockSaver/smart-saving-contract/blob/master/SmartSavingContract/SmartSavingContract.cs)
   * ExecutionEngine.ExecutingScriptHash
   * JSON Arrays
   * Storage - medium-high level
   * Assets and Asset IDs
5. [imusify/smart-contract-incentify](https://github.com/imusify/smart-contract-incentify/blob/master/contract/ImusifyToken.cs) from [https://github.com/imusify/smart-contract-incentify/blob/master/contract/ImusifyToken.cs](https://github.com/imusify/smart-contract-incentify/blob/master/contract/ImusifyToken.cs)
    * NEP5 token
    * Storage - medium
    * CheckWitness(owner) - (commented out) owner account in storage
6. [mmoravec/luckyneo](https://github.com/mmoravec/luckyneo/blob/master/LuckyNeo.py) from [https://github.com/mmoravec/luckyneo/blob/master/LuckyNeo.py](https://github.com/mmoravec/luckyneo/blob/master/LuckyNeo.py)
7. [birmas/neotrade](https://github.com/birmas/neotrade/blob/master/neotrade.cs) from [https://github.com/birmas/neotrade/blob/master/neotrade.cs](https://github.com/birmas/neotrade/blob/master/neotrade.cs)
    * NEP5 token
    * Assets and Asset IDs
    * Storage - medium level
    * Admin account
    * Runtime.CheckWitness
    * VerifySignature (commented out)
    * ExecutionEngine.ExecutingScriptHash
    * Transaction
    * Blockchain.GetHeader - for discount rate
8. [nickazg/neo-fund](https://github.com/nickazg/neo-fund/blob/master/neo-fund-sc/neo-fund-sc/NeoFund.cs) from [https://github.com/nickazg/neo-fund/blob/master/neo-fund-sc/neo-fund-sc/NeoFund.cs](https://github.com/nickazg/neo-fund/blob/master/neo-fund-sc/neo-fund-sc/NeoFund.cs)
    * Transaction - high level
    * Role-based rights management
    * Storage - medium-high level
    * Assets and Asset IDs
    * Blockchain.GetHeader(Blockchain.GetHeight()).Timestamp
9. [ambethia/neo-raffle](https://github.com/ambethia/neo-raffle/blob/master/Contract.cs) from [https://github.com/ambethia/neo-raffle/blob/master/Contract.cs](https://github.com/ambethia/neo-raffle/blob/master/Contract.cs)
    * !Runtime.CheckWitness(Owner)
    * ExecutionEngine.ExecutingScriptHash
    * Blockchain - high level
    * Transaction - high level
    * Assets and Asset IDs
    * long randomNumber = (long)(header.ConsensusData >> 32);
    * var prevTx = Blockchain.GetTransaction(input.PrevHash);
    * var thisOutput = prevTx.GetOutputs()[input.PrevIndex];
10. [block-shaman/NepSwap](https://github.com/block-shaman/NepSwap/blob/master/Contract1.cs) from [https://github.com/block-shaman/NepSwap/blob/master/Contract1.cs](https://github.com/block-shaman/NepSwap/blob/master/Contract1.cs)
    * ExecutionEngine.ScriptContainer
    * Transaction - high level
    * Blockchain.GetAccount(contractHash) - hardcoded contractHash
    * NEP1 template
    * Assets and AssetIDs
    * ExecutionEngine.ExecutingScriptHash
11. [MediaServe/KRYPTON](https://github.com/MediaServe/KRYPTON/blob/master/contract/krypton.py) from [https://github.com/MediaServe/KRYPTON/blob/master/contract/krypton.py](https://github.com/MediaServe/KRYPTON/blob/master/contract/krypton.py)
12. [Relfos/phantasma](https://github.com/Relfos/phantasma/blob/master/PhantasmaContract/PhantasmaContract.cs) from [https://github.com/Relfos/phantasma/blob/master/PhantasmaContract/PhantasmaContract.cs](https://github.com/Relfos/phantasma/blob/master/PhantasmaContract/PhantasmaContract.cs)
    * NEP token
    * Assets and AssetIDs
    * ExecutionEngine.ExecutingScriptHash
    * Blockchain.GetHeader(Blockchain.GetHeight()).Timestamp
    * "Secure Blockchain email service"
    * Elaborate but good smart contract
13. [SmartPromise/SmartPromise.NeoContract](https://github.com/SmartPromise/SmartPromise.NeoContract/blob/master/SmartPromise/SmartPromise.cs) from [https://github.com/SmartPromise/SmartPromise.NeoContract/blob/master/SmartPromise/SmartPromise.cs](https://github.com/SmartPromise/SmartPromise.NeoContract/blob/master/SmartPromise/SmartPromise.cs)
    * Storage - medium level
    * NEP token
    * ExecutionEngine.ExecutingScriptHash
    * Transactions - high level
    * Assets and AssetIDs
14. [JorritvandenBerg/sunny-dapp](https://github.com/JorritvandenBerg/sunny-dapp/blob/master/smartcontract/sunny_dapp.py) from [https://github.com/JorritvandenBerg/sunny-dapp/blob/master/smartcontract/sunny_dapp.py](https://github.com/JorritvandenBerg/sunny-dapp/blob/master/smartcontract/sunny_dapp.py)
15. [ConjurTech/switcheo](https://github.com/ConjurTech/switcheo/blob/master/switcheo/BrokerContract.cs) from [https://github.com/ConjurTech/switcheo/blob/master/switcheo/BrokerContract.cs](https://github.com/ConjurTech/switcheo/blob/master/switcheo/BrokerContract.cs)
    * Transaction - high level
    * Elaborate and long - good
    * Assets and AssetIDs
    * !Runtime.CheckWitness(offer.MakerAddress)
    * Long but very factored
16. [xtolya/TripShares](https://github.com/xtolya/TripShares/blob/master/TripShareSmartContract/TripShareSmartContract/TripShareContract.cs) from [https://github.com/xtolya/TripShares/blob/master/TripShareSmartContract/TripShareSmartContract/TripShareContract.cs](https://github.com/xtolya/TripShares/blob/master/TripShareSmartContract/TripShareSmartContract/TripShareContract.cs)
    * Transaction - high level
    * Elaborate and long - good
    * Assets and AssetIDs
    * NEP5
17. [Nikolaj-K/turing-complete-smart-contract](https://github.com/Nikolaj-K/turing-complete-smart-contract/blob/master/contract.cs) from [https://github.com/Nikolaj-K/turing-complete-smart-contract/blob/master/contract.cs](https://github.com/Nikolaj-K/turing-complete-smart-contract/blob/master/contract.cs)
    * Cool app

Figure C.1. First dApps Competition: List of Smart Contracts

## References

* [DAPPSCOMPETE] Chris Hager, [CoZ first dApps competition dApp review](https://medium.com/proof-of-working/coz-first-dapps-competition-dapp-review-3a6b284afaef) from [https://medium.com/proof-of-working/coz-first-dapps-competition-dapp-review-3a6b284afaef](https://medium.com/proof-of-working/coz-first-dapps-competition-dapp-review-3a6b284afaef), Nov 23, 2017


