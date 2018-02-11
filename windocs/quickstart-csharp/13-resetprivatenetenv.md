# NEO Blockchain Quick Start Process for .NET Developers

NEO Blockchain Documentation for .NET Developers ([url](https://github.com/mwherman2000/neo-windocs/tree/master/windocs))

## Appendix C - Reset your NEO privatenet environment: Container, Wallets, and Clients

### Purpose

The purpose of this section is to document how to reset your NEO privatenet environment: container and clients; for example, when you run out of gas.

### Goals, Non-Goals and Assumptions

* Being able to reset your NEO privatenet environment as quickly as possible

### Principles

* Provide reliable documentation: timely, accurate, visual, and complete
* Save as much of a person's time as possible
* Use open source software whenever possible

### Drivers

* Need in the NEO .NET developer community to have concise and easy-to-follow documentation to enable people to get up to speed developing NEO smart contracts in as short a time as possible

## Stop all of your NEO Client apps

1. Stop all of your NEO client apps that may be using the NEO Docker container (e.g. neo-cli, neo-gui, ...).

## Reset your NEO privatenet Docker container

2. Reset the the NEO Docker container by running the following script: 
    ```
    docker stop neo-privnet-with-gas
    docker container list
    docker start neo-privnet-with-gas
    docker container list
    pause
    ```
    Script: NEO Docker Restart ([./scripts/neodockerrestart.bat.txt](./scripts/neodockerrestart.bat.txt))

## Reset your NEO privatenet wallets

3. Delete all of your wallets you used with the NEO privatenet. They will need to be recreated anyway.

**NOTE:** **Be very careful** to only delete wallets used with the NEO **privatenet**.

## Reset your NEO privatenet clients

4. Delete all of your client app's blockchain database folders.
5. Delete all of your client app's `peers.dat` files.
6. If it is a Visual Studio development project, delete the entire `bin/Debug` folder.

## Start your NEO privatenet client apps

7. After the preceding tasks are complete, the reset is complete. You can rebuild/start your NEO privatenet client apps.

## References

* N/A
