# C#.NEO Smart Contract Developers Guide

NEO Blockchain Documentation for .NET Developers ([url](https://github.com/mwherman2000/neo-windocs/tree/master/windocs))

## Purpose

The purpose of this document is capture the knowledge and best practices for C# smart contract development on the NEO Blockchain platform.

This document is specifically targeted at .NET developers and architects. 

### Caveat

In addition, when the first version of the document was written (February 2018), you will also need to have an [*early adopters*](https://en.wikipedia.org/wiki/Technology_adoption_life_cycle) mind set. It's the early days. You'll be downloading the code for most of the developer tools (aside from Visual Studio) and compiling them yourself. It may not always be fun but I promise it will certainly be rewarding in the end.

## Goals

* Capture basic as well as advanced knowledge related to developing C# smart contracts across the application lifecyle (ALM)
    * Requirements
    * NEO C# Language Considerations
    * NEO System Fees
    * Design Patterns
    * Creating Secure Contracts
    * Implementation
    * Deployment
    * Testing
    * Maintenance
    * Documentation
* Capture recommended best practices for C# smart contract development
* Non-goal: This scope of this document is limited to smart contract development only - not the other components and services of the [NEO Blockchain](../quickstart-csharp/README.md) platform.

## Principles

* Provide reliable documentation: timely, accurate, visual, and complete
* Save as much of a person's time as possible
* Use open source software whenever possible

## Drivers

* Need in the NEO .NET developer community to have concise and easy-to-follow documentation to enable people to get up to speed developing NEO smart contracts in as short a time as possible

## Sections

1. [Requirements](./01-requirements.md)
2. [NEO C# Language Considerations](./02-csharp.md)
3. [NEO System Fees](./03-systemfees.md)
4. [Design Patterns](./04-designpatterns.md)
5. [Writing Secure Contracts](./05-securecontracts.md)
6. [Implementation](./06-implementation.md)
7. [Deployment](./07-deployment.md)
8. [Testing](./08-testing.md)
9. [Maintenance](./09-maintenance.md)
10. [Documentation](./10-documentation.md)
11. [Appendix A - NEO Object Model Overview](./11.neoobjectmodel.md)
12. [Appendix B - Roadmap](./12-roadmap.md)
12. [Appendix C - Sample Smart Contracts](./13-samplesmartcontracts.md)

## References

* [MSCODINGGUIDE] Microsoft, [C# Coding Conventions (C# Programming Guide)](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions) from [https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/inside-a-program/coding-conventions)
    > The C# Language Specification does not define a coding standard. However, the guidelines in this topic are used by Microsoft to develop samples and documentation. 

    > Coding conventions serve the following purposes:

    > * They create a consistent look to the code, so that readers can focus on content, not layout.

    > * They enable readers to understand the code more quickly by making assumptions based on previous experience.

    > * They facilitate copying, changing, and maintaining the code.

    > * They demonstrate C# best practices.

* [FRAMEWORKGUIDLINES] Microsoft, [Framework Design Guidelines](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/) from [https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/)
    > This section provides guidelines for designing libraries that extend and interact with the .NET Framework. ...

    > The guidelines are organized as simple recommendations prefixed with the terms Do, Consider, Avoid, and Do not. 

    >These guidelines are excerpted from the book Framework Design Guidelines: Conventions, Idioms, and Patterns for Reusable .NET Libraries, 2nd Edition, by Krzysztof Cwalina and Brad Abrams.

* [ETHCONCENSYSSECURITY] Concensys, [Smart Contract Security Best Practices (Ethereum)](https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md) from [https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md](https://github.com/ConsenSys/smart-contract-best-practices/blob/master/README.md)

* [ETHSTYLEGUIDE] Solidity project, [Style Guide (Ethereum)](http://solidity.readthedocs.io/en/latest/style-guide.html) from [http://solidity.readthedocs.io/en/latest/style-guide.html](http://solidity.readthedocs.io/en/latest/style-guide.html)

* [ETHPATTERNS] Solidity project, [Common Patterns](http://solidity.readthedocs.io/en/latest/common-patterns.html) from [http://solidity.readthedocs.io/en/latest/common-patterns.html](http://solidity.readthedocs.io/en/latest/common-patterns.html)

* [ETHSECURITY] Solidity project, [Security Considerations](http://solidity.readthedocs.io/en/latest/security-considerations.html) from [http://solidity.readthedocs.io/en/latest/security-considerations.html](http://solidity.readthedocs.io/en/latest/security-considerations.html)

## Other Good Resources

* TODO


