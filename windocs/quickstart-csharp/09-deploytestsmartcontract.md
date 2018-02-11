# NEO Blockchain Quick Start Process for .NET Developers

NEO Blockchain Documentation for .NET Developers ([url](https://github.com/mwherman2000/neo-windocs/tree/master/windocs))

## Activity 9 - Deploy and test HelloWorld smart contract

TODO

### Purpose

The purpose of this activity is to use deploy and test the HelloWorld smart contract created in the previous activity. It uses the the neo-gui-developer tool that was build in an earlier activity. This activity also uses the NEO Docker container that was installed and configured also in an earlier activity.

### Goals, Non-Goals and Assumptions

* Ensure you have a working and properly configured set of NEO developer tools for creating and building smart contracts in Visual Studio with the C# programming language

### Principles

* Provide reliable documentation: timely, accurate, visual, and complete
* Save as much of a person's time as possible
* Use open source software whenever possible

### Drivers

* Need in the NEO .NET developer community to have concise and easy-to-follow documentation to enable people to get up to speed developing NEO smart contracts in as short a time as possible

## Start the NEO privatenet Docker container

1. Start the NEO privatenet Docker container by opening PowerShell and running the following commands: 
    ```
    docker container list
    docker start neo-privnet-with-gas
    docker container list
    pause
    ```
    Script: NEO Docker Start  ([./scripts/neodockerstart.bat.txt](./scripts/neodockerstart.bat.txt))

    The script produces the following output:

    ![NEO Docker Start](./images/07-installneoprivatenetcontainer/DockerNeo1Start.png)
  
    Figure 9.1. NEO Docker Start

## Test the NEO privatenet Docker Container

2. To test the NEO Docker container, run following script:
    ```
    REM cd opt/neo-python
    REM python3 prompt.py -p
    REM block 0
    docker exec -it neo-privnet-with-gas /bin/bash
    pause
    ```
    Script: NEO Docker Python CLI/Shell ([./scripts/neodockerpshell.bat.txt](./scripts/neodockerpshell.bat.txt))

## Configure `neo-gui (developer)` to use the NEO privatenet Docker container

3. Open Windows Explorer and navigate to `TODO`:

    ![`neo-gui (developer)` bin/Debug Folder](./images/07-installneoprivatenetcontainer/DockerNeo1Start.png)

    Figure 9.2. `neo-gui (developer)` bin/Debug Folder

4. Configure `neo-gui (developer)` by replacing the 2 JSON configuration files with the contents of the following JSON files:

* config.json: ([./json/config.neodocker.json](./json/config.neodocker.json))
* protocol.json: ([./json/protocol.neodocker.json](./json/protocol.neodocker.json))

5. In addition, make sure you:
* Delete your old blockchain database folder
* Delete your old `peers.dat` file

6. TODO
* Start neo-gui.exe

7. TODO
* Re-index your database

8. Create a new wallet using the WIF key provided with the NEO Docker container documentation [NEODOCKER1](https://hub.docker.com/r/metachris/neo-privnet-with-gas/#Wallet). 
    ```
    WIF key: KxDgvEKzgSBPPfuVfw67oPQBSjidEiqTHURKSDL1R7yGaGYAeYnr
    Address: AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y
    ```

## Use `neo-gui (developer)` to deploy the HelloWorld smart contract

1. TODO

1. TODO

1. TODO

## Use `neo-gui (developer)` to invoke and test the HelloWorld smart contract

1. TODO

1. TODO

    Parameter/Return&nbsp;Type | Description |
    :--------|:---------------------- |
    Signature|00|
    Boolean|01|
    Integer|02|
    Hash160 (160-bit hash value)|03|
    Hash256 (256-bit hash value)|04|
    ByteArray|05|
    PublicKey|06|
    String|07|
    Array|10|
    InteropInterface|f0|   
    Void|ff|


1. TODO

The tasks for this activity are complete. Proceed to [Activity 10 - Celebrate](./10-celebrate.md).

## Script Library

* NEO Docker Start ([./scripts/neodockerstart.bat.txt](./scripts/neodockerstart.bat.txt))

## References

* [NEOTUTORIAL] NEO Project, [NEO smart contract tutorial](http://docs.neo.org/en-us/sc/tutorial.html) from [http://docs.neo.org/en-us/sc/tutorial.html](http://docs.neo.org/en-us/sc/tutorial.html)
* [NEODOCKER1] metachris, [metachris/neo-privnet-with-gas](https://hub.docker.com/r/metachris/neo-privnet-with-gas/) from [https://hub.docker.com/r/metachris/neo-privnet-with-gas/]https://hub.docker.com/r/metachris/neo-privnet-with-gas/()
