# Quick Start Process Guide for Microsoft .NET Developers

NEO Blockchain documentation for Microsoft .NET Developers ([url](https://github.com/mwherman2000/neo-windocs/tree/master/windocs))

## Activity 0 - Prerequisites and Recommendations

### Purpose

The purpose of this activity is to for you to ensure you have Windows environment that is compatible with the list of 10 activities described in this document (and to save you a lot of time if your environment isn't compatible).  

### Goals, Non-Goals and Assumptions

The goal of this activity is to inform you about the minimum and recommended pre-requisites for successful execution of the remaining acitivities in Quick Start Process Guide for Windows .NET Developers.

### Principles

* Provide reliable documentation
* Save as much of a person's time as possible

### Drivers

* Lack of an existing set of concise and easy to follow documentation

## Prerequisites and Recommendations

The basic hardware and software prerquisites are that you have a computer (PC or laptap) with:
* Microsoft Windows 10 operating system (any edition - Home or Pro or Academic)
* Latest Windows Updates installed
* 8GB of RAM (16GM or more prefered because you need to install and enable the Hyper-V feature and service)
* 50GB of free disk space (100GB ore preferred because you will eventually have multiple copies of the NEO blockchain files downloaded on to your machine)
* An SSD (solid state drive) is preferred over a conventional hard drive (HDD) for perfomance reasons but it's not a necessity

The activities in this document were tested on two configurations:
* Windows 10 Home edition HP laptop, 8GB RAM, 1TB HDD, Intel i5 processor
* Windows 10 Pro edition Levnovo laptop, 32GB RAM, 500GB SSD + 500GB HDD, Intel i7 processor

## Download and Install the Microsoft .NET 4.7 Developer Pack

The .NET 4.7 Dev Pack is required to be able to build some components in the NEO developer toolset. If you overlook this step, Visual Studio will interupt and prompt to install this dev pack when it is required.

1. Download the .NET 4.7 Dev Pack starting here: [https://support.microsoft.com/en-ca/help/3186612/the-net-framework-4-7-developer-pack-and-language-packs](https://support.microsoft.com/en-ca/help/3186612/the-net-framework-4-7-developer-pack-and-language-packs)

![Microsoft Knowlege Base: The .NET Framework 4.7 Developer Pack and Language Packs](./images/00-prerequisites/Dotnet4-7DevPack1Install.png)
Figure 0.1. Microsoft Knowlege Base: The .NET Framework 4.7 Developer Pack and Language Packs

2. This will take you to the Microsoft Downloads site for the dev pack: [https://www.microsoft.com/en-us/download/details.aspx?id=55168](https://www.microsoft.com/en-us/download/details.aspx?id=55168). Scroll down and click the Download button to download the installer executable. 

![Microsoft Downloads site: Microsoft .NET Framework 4.7 Developer Pack and Language Packs for Windows 7 SP1, Windows 8.1, Windows 10 Anniversary Update, Windows Server 2008 R2 SP1, Windows Server 2012, Windows Server 2012 R2 and Windows Server 2016](./images/00-prerequisites/Dotnet4-7DevPack2Install.png)
Figure 0.2. Microsoft Downloads site: Microsoft .NET Framework 4.7 Developer Pack and Language Packs for Windows 7 SP1, Windows 8.1, Windows 10 Anniversary Update, Windows Server 2008 R2 SP1, Windows Server 2012, Windows Server 2012 R2 and Windows Server 2016

3. Go to your Downloads folder on your computer and double-click the `NDP47-DevPack-KB3186612-ENU.exe` executable.
4. Click OK to run as Adminstrator for the installation process.

![.NET 4.7 Dev Pack EULA](./images/00-prerequisites/Dotnet4-7DevPack3Install.png)
Figure 0.3. .NET 4.7 Dev Pack EULA

4. The install process will start.

![v](./images/00-prerequisites/Dotnet4-7DevPack4Install.png)
Figure 0.4. c

5. The following page will be displayed when the installation is complete.

![.NET 4.7 Dev Pack Installation Complete](./images/00-prerequisites/Dotnet4-7DevPack5Install.png)
Figure 0.5. .NET 4.7 Dev Pack Installation Complete

6. Proceed to [Activity 1 - Download and install Visual Studio 2017 Community Edition integrated development environment (IDE)](01-installvisualstudio.md).

## References

* [DevPack1] [The .NET Framework 4.7 Developer Pack and Language Packs](https://support.microsoft.com/en-ca/help/3186612/the-net-framework-4-7-developer-pack-and-language-packs) from [https://support.microsoft.com/en-ca/help/3186612/the-net-framework-4-7-developer-pack-and-language-packs](https://support.microsoft.com/en-ca/help/3186612/the-net-framework-4-7-developer-pack-and-language-packs)
* [DevPack2] [Microsoft .NET Framework 4.7 Developer Pack and Language Packs for Windows 7 SP1, Windows 8.1, Windows 10 Anniversary Update, Windows Server 2008 R2 SP1, Windows Server 2012, Windows Server 2012 R2 and Windows Server 2016](https://www.microsoft.com/en-us/download/details.aspx?id=55168) from [https://www.microsoft.com/en-us/download/details.aspx?id=55168](https://www.microsoft.com/en-us/download/details.aspx?id=55168)
