# ERC

ERC(Ethereum Request for Comments) is a technical standard used in the Ethereum ecosystem to define how smart contracts should work.


## ERC-20 Token Standard

### What is a Token?

Tokens can represent virtually anything in Ethereum:

    - reputation points in an online platform
    - skills of a character in a game
    - financial assets like a share in a company
    - a fiat currency like USD
    - an ounce of gold
    - and more...


The ERC-20 introduces a standard for [Fungible](https://www.merriam-webster.com/dictionary/fungible) Tokens, in other words, they have a property that makes each Token be exactly the same (in type and value) as another Token. For example, an ERC-20 Token acts just like the ETH, meaning that 1 Token is and will always be equal to all the other Tokens. 

Source: [ethereum](https://ethereum.org/developers/docs/standards/tokens/erc-721/)

## ERC-721 Non-Fungible Token Standard

### What is a Non-Fungible Token?

A Non-Fungible Token (NFT) is used to identify something or someone in a unique way. This type of Token is perfect to be used on platforms that offer collectible items, access keys, lottery tickets, numbered seats for concerts and sports matches, etc.

The ERC-721 introduces a standard for NFT, in other words, this type of Token is unique and can have different value than another Token from the same Smart Contract, maybe due to its age, rarity or even something else like its visual. Wait, visual?

Yes! All NFTs have a uint256 variable called tokenId, so for any ERC-721 Contract, the pair contract address, uint256 tokenId must be globally unique. That said, a dapp can have a "converter" that uses the tokenId as input and outputs an image of something cool, like zombies, weapons, skills or amazing kitties!
