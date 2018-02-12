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

## Start (reset) the NEO privatenet Docker container

1. Start the NEO privatenet Docker container by opening PowerShell and running the following commands: 
    ```
    docker container list
    docker stop neo-privnet-with-gas
    docker container list
    docker rm neo-privnet-with-gas
    docker container list
    docker run -d --name neo-privnet-with-gas -p 20333-20336:20333-20336/tcp -p 30333-30336:30333-30336/tcp metachris/neo-privnet-with-gas
    docker container list
    pause
    ```
    Script: NEO Docker Reset ([./scripts/neodockerreset.bat.txt](./scripts/neodockerreset.bat.txt))

    The script produces the following output:

    ![NEO Docker Reset](./images/07-installneoprivatenetcontainer/DockerNeo1Reset.png)
  
    Figure 9.1. NEO Docker Reset

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

3. Open Windows Explorer and navigate to `C:\NEO\neo-gui-developer\neo-gui\bin` and right-click on the the `Debug` folder and delete it (and all of of the folder's contents). 

    ![C:\NEO\neo-gui-developer\neo-gui\bin](./images/09-deploytestsmartcontract/HelloWorld0aTest.png)

    Figure 9.2. C:\NEO\neo-gui-developer\neo-gui\bin

4. Navigate to `C:\NEO\neo-gui-developer`.

    ![C:\NEO\neo-gui-developer](./images/09-deploytestsmartcontract/HelloWorld0bTest.png)

    Figure 9.3. C:\NEO\neo-gui-developer

5. Double-click `neo-gui.sln` to open the `neo-gui-developer` project in Visual Studio.

    ![Visual Studio: neo-gui project](./images/09-deploytestsmartcontract/HelloWorld0cTest.png)

    Figure 9.4. Visual Studio: neo-gui project

6. In Visual Studio, replace the contents of `config.json` with the contents of `config.neodocker.json`.

    ![Visual Studio: config.json](./images/09-deploytestsmartcontract/HelloWorld0cTest.png)

    Figure 9.5. Visual Studio: config.json

    **NOTE:** If `config.neodocker.json` is not part of your project, you can download it from [here](./json/config.neodocker.json) ([./json/config.neodocker.json](./json/config.neodocker.json)) and place it in the `C:\NEO\neo-gui-developer\neo-gui` folder. Right-click on the `neo-gui` project folder in Visual Studio and select `Add` > `Existing Item...` > `*.*`. Select `config.neodocker.json` and click `Add`.

7. Similarly, replace the contents of `protocol.json` with the contents of `protocol.neodocker.json`.

    ![Visual Studio: protocol.json](./images/09-deploytestsmartcontract/HelloWorld0dTest.png)

    Figure 9.6. Visual Studio: protocol.json

    **NOTE:** If `protocol.neodocker.json` is not part of your project, you can download it from [here](./json/protocol.neodocker.json) ([./json/protocol.neodocker.json](./json/protocl.neodocker.json)) and place it in the `C:\NEO\neo-gui-developer\neo-gui` folder. Right-click on the `neo-gui` project folder in Visual Studio and select `Add` > `Existing Item...` > `*.*`. Select `protocol.neodocker.json` and click `Add`.

8. In Visual Studio, click `Start` to rebuild and start `neo-gui`. It should starting syncing with the NEO privatenet Docker container.

    ![neo-gui: Running against the NEO privatenet Docker container](./images/09-deploytestsmartcontract/HelloWorld2Test.png)

    Figure 9.7. neo-gui: Running against the NEO privatenet Docker container

    **NOTE:** If you made the optional code change in Activity 5 - Build and test NEO developer tool projects (from source), you will see the name of your NEO blockchain folder in the title bar (e.g. DockerChainTestNet).

## Create a new development wallet

9. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldATest.png)

    Figure 9.X. XXX

10. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldBTest.png)

    Figure 9.X. XXX

11. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldCTest.png)

    Figure 9.X. XXX

12. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldDTest.png)

    Figure 9.X. XXX

13. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldETest.png)

    Figure 9.X. XXX

## Import the existing Developer account from the NEO privatenet Docker container

14. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldFTest.png)

    Figure 9.X. XXX

15. Enter the WIF key provided with the NEO Docker container documentation [NEODOCKER1](https://hub.docker.com/r/metachris/neo-privnet-with-gas/#Wallet). 
    ```
    WIF key: KxDgvEKzgSBPPfuVfw67oPQBSjidEiqTHURKSDL1R7yGaGYAeYnr
    ```

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldGTest.png)

    Figure 9.X. XXX

16. The result should be that you've created the following second account at address:
    ```
    Address: AK2nJJpJr6o664CWJKi1QRXjqeic2zRp8y
    ```

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldHTest.png)

    Figure 9.X. XXX

## Deploy your smart contract (HelloWorld 1.0)

17. Open Visual Studio 2017 to create a new NEO smart contract project.

    ![Visual Studio 2017](./images/05-buildneodevtools/NeonCompilerLTest.png)

    Figure 9.x. Visual Studio 2017

18. Select `File` > `New` > `Project...` to open the New Project dialog box. Select `Visual C#`. Select `NeoContract`. Click `OK` to close this dialog box and create a new NeoContract solution and project in Visual Studio. 

    ![Visual Studio: Create a New NeoContract Project](./images/05-buildneodevtools/NeonCompilerMTest.png)

    Figure 9.x. Visual Studio: Create a New NeoContract Project

    **NOTE:** If you have created previous NeoContract projects, your project may be called `NeoContract2`, `NeoContract3`, or whatever you chose to name the project.  Remember the project name and path because you will need to find the AVM file later on in this activity.

19. Visual Studio may take a few minutes to create the NeoContract project.

    ![Visual Studio: Creating the NeoContract Project](./images/05-buildneodevtools/NeonCompilerNTest.png)

    Figure 9.x. Visual Studio: Creating the NeoContract Project

20. Right-click on the NeoContract project folder and select `Build`. Note the highlighted messages in the Build section of the Output panel. These 2 message indicate the Visual Studio was able to create both the NEO virtual machine byte code file as well as the Application Binary Interace (ABI) file (in JSON format).

    **NOTE:** If you don't see these 2 messages, the most likely senarios are:
      * `noen.dll` wasn't published properly. Go back to Task 6 of this activity.
      * The `Path` environment variable was not set correctly. Go back to Task 16 of this activity.
      * You had opened Visual Studio before you set the `Path` environment variable.  Close Visual Studio and then go back to Task 20.

    ![Visual Studio: Building the NeoContract Project](./images/05-buildneodevtools/NeonCompilerOTest.png)

    Figure 9.x. Visual Studio: Building the NeoContract Project

## Deploy your first smart contract

17. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldITest.png)

    Figure 9.X. XXX

18. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldJTest.png)

    Figure 9.X. XXX

# Invoke your first smart contract

19. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldKTest.png)

    Figure 9.X. XXX

20. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldLTest.png)

    Figure 9.X. XXX

21. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldMTest.png)

    Figure 9.X. XXX

22. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldNTest.png)

    Figure 9.X. XXX

23. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldOTest.png)

    Figure 9.X. XXX

24. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldPTest.png)

    Figure 9.X. XXX

25. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldQTest.png)

    Figure 9.X. XXX

26. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldRTest.png)

    Figure 9.X. XXX

## Create your second smart contract (HelloWorld 2.0)

26. Follow the previous tasks to create a new NeonContract project (e.g. NeoContract2).

    **NOTE:** If you have created previous NeoContract projects, your project may be called `NeoContract3`, `NeoContract4`, or whatever you chose to name the project.  Remember the project name and path because you will need to find the AVM file later on in this activity.

## Deploy your second smart contract

27. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldSTest.png)

    Figure 9.X. XXX

32. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldTTest.png)

    Figure 9.X. XXX
33. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldUTest.png)

    Figure 9.X. XXX

34. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldVTest.png)

    Figure 9.X. XXX

35. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldWTest.png)

    Figure 9.X. XXX

36. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldXTest.png)

    Figure 9.X. XXX

37. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldYTest.png)

    Figure 9.X. XXX

38. TODO

    ![XXX](./images/09-deploytestsmartcontract/HelloWorldZTest.png)

    Figure 9.X. XXX


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


The tasks for this activity are complete. Proceed to [Activity 10 - Celebrate](./10-celebrate.md).

## Script Library

* NEO Docker Start ([./scripts/neodockerstart.bat.txt](./scripts/neodockerstart.bat.txt))

## References

* [NEOTUTORIAL] NEO Project, [NEO smart contract tutorial](http://docs.neo.org/en-us/sc/tutorial.html) from [http://docs.neo.org/en-us/sc/tutorial.html](http://docs.neo.org/en-us/sc/tutorial.html)
* [NEODOCKER1] metachris, [metachris/neo-privnet-with-gas](https://hub.docker.com/r/metachris/neo-privnet-with-gas/) from [https://hub.docker.com/r/metachris/neo-privnet-with-gas/]https://hub.docker.com/r/metachris/neo-privnet-with-gas/()

## Other Good Resources

* [NEOPYTHONTUTORIAL] Nick Fujita, [NEO Smart Contracts Tutorial: helloWorld (Python)](https://steemit.com/neo/@z0yo/neo-smart-contracts-tutorial-helloworld) from [https://steemit.com/neo/@z0yo/neo-smart-contracts-tutorial-helloworld](https://steemit.com/neo/@z0yo/neo-smart-contracts-tutorial-helloworld)
* [NEOPYTHONTUTORIALVIDEO] Nick Fujita, [NEO Smart Contract Tutorial - Hello World (Python)](https://www.youtube.com/watch?v=9Ha_5RdOQrA) from [https://www.youtube.com/watch?v=9Ha_5RdOQrA](https://www.youtube.com/watch?v=9Ha_5RdOQrA)
* [NEOGUIDEVPULL38] Michael Herman. [Pull Request #38 to have the `config.neodocker.json` and `protocol.neodocker.json` files added to the `neo-gui-developer` project](https://github.com/CityOfZion/neo-gui-developer/pull/38) from [https://github.com/CityOfZion/neo-gui-developer/pull/38](https://github.com/CityOfZion/neo-gui-developer/pull/38)
