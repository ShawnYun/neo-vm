<p align="center">
<a href="https://neo.org/">
      <img
      src="https://neo3.azureedge.net/images/logo%20files-dark.svg"
      width="250px" alt="neo-logo">
  </a>
</p>


<p align="center">
  <a href="https://travis-ci.com/neo-project/neo-vm">
    <img src="https://travis-ci.com/neo-project/neo-vm.svg?branch=master" alt="Current TravisCI build status.">
  </a>
  <a href="https://github.com/neo-project/neo-vm/releases">
    <img src="https://badge.fury.io/gh/neo-project%2Fneo-vm.svg" alt="Current neo-vm version.">
  </a>
  <a href='https://coveralls.io/github/neo-project/neo-vm'>
    <img src='https://coveralls.io/repos/github/neo-project/neo-vm/badge.svg' alt='Coverage Status' />
  </a>
  <a href="https://github.com/neo-project/neo-vm">
    <img src="https://tokei.rs/b1/github/neo-project/neo-vm?category=lines" alt="total lines.">
  </a>
  <a href="https://github.com/neo-project/neo-vm/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License.">
  </a>	
</p>

# NEO Virtual Machine


## Table of Contents
1. [Overview](#overview)
2. [Project structure](#project-structure)
3. [Related projects](#related-projects)
4. [Bounty program](#bounty-program)
5. [License](#license)


## Overview
This is the virtual machine of NEO: **NeoVM**.

For detailed documentation, see [docs.neo.org](https://docs.neo.org/docs/en-us/index.html) and the [NEO whitepaper](https://docs.neo.org/docs/en-us/basic/whitepaper.html).



## Project structure
An overview of the project folders can be seen below.

|Folder|Content|
|---|---|
|Types| The basic data types used by NeoVM.|
|Debugger|The Debugger of NeoVM.|
|EvaluationStack|Basic operation of EvaluationStack|
|ExecutionContext|Classes used to store Script, EvaluationStack and    Slot.|
|ExecutionEngine|Specific operations for each OpCode.|
|OpCode|All opcodes supported by NeoVM.|
|ScriptBuilder|Classes used to build a NeoVM script.|
|Slot|StaticFields, LocalVariables and Arguments are stored in Slot.|
|VMState|There are 4 states of NeoVM: NONE, HALT, FAULT, BREAK.|


## Related projects
Code references are provided for all platform building blocks. That includes the base library, the VM, a command line application and the compiler. 

* [neo:](https://github.com/neo-project/neo/) Neo core library, contains base classes, including ledger, p2p and IO modules.
* [neo-vm:](https://github.com/neo-project/neo-vm/) Neo Virtual Machine is a decoupled VM that Neo uses to execute its scripts. It also uses the `InteropService` layer to extend its functionalities.
* [neo-node:](https://github.com/neo-project/neo-node/) Executable version of the Neo library, exposing features using a command line application or GUI.
* [neo-modules:](https://github.com/neo-project/neo-modules/) Neo modules include additional tools and plugins to be used with Neo.
* [neo-devpack-dotnet:](https://github.com/neo-project/neo-devpack-dotnet/) These are the official tools used to convert a C# smart-contract into a *neo executable file*.

## Bounty program
You can be rewarded by finding security issues. Please refer to our [bounty program page](https://neo.org/bounty) for more information.

## License
The NEO project is licensed under the [MIT license](LICENSE).