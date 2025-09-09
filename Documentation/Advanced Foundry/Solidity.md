# Solidity


## Table of Contents
 - [Introduction](#introduction)
 - [Smart Contract](#what-is-a-smart-contract)
 - [First Example](#first-example)





## Introduction

To build any smart contract you should have a little of understanding about Solidity, bellow is a small tutorial of the language but i recomend you to read [the documentation](https://docs.soliditylang.org/en/latest/)

## What is a Smart Contract

Smart contracts are digital contracts stored on a blockchain that are automatically executed when predetermined terms and conditions are met.

It is ok if this defenition doesn't tell you anything, we will go into more details later.

## First example

Let's create the simplest example, a Simple Storage.

```Solidity
// SPDX-License-Identifier: GPL-3.0
pragma solidity >=0.4.16 <0.9.0;

contract SimpleStorage {
    uint storedData;

    function set(uint x) public {
        storedData = x;
    }

    function get() public view returns (uint) {
        return storedData;
    }
}
```

The first line in this code block is not stricly required, but it's strongly recomended. It is a license identifier that tells users, developers and auditors the legal terms under which the code can be used, modified and redistributed.

The next line specifies the range of versions that this Solidity code was written. This is done inorder to ensure the right compiler version.

A Contract in Solidity has a similar structure to a class in Java/C++. The Contract has a some data (its State) and a collection of code (its functions) that resides in a specific address on the Ethereum blockchain.

Solidity is a strictly typed language, that mean that whenever you want to create a variable it's type needs to be specified `uint storedData`

Check out [this example](./Solidity-Example) with some extra features
