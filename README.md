# AVALANCHE-MODULE3-PROJECT
**MyToken - JAYAXP Token**

**Overview:**

MyToken is a custom ERC-20 token with the symbol "JAYAXP". It is based on the Ethereum blockchain and follows the ERC-20 standard, which allows it to be compatible with various decentralized applications (DApps), wallets, and exchanges that support ERC-20 tokens.

**License:**

This contract is released under the MIT License, which is a permissive open-source license that allows anyone to use, modify, and distribute the code under certain conditions. You can find the full text of the license in the comments of the contract, indicated by the SPDX-License-Identifier: MIT tag.

**Features:**

1. **ERC20:** The contract inherits from the `ERC20` contract provided by OpenZeppelin. This base contract includes all the standard functions and events required for an ERC-20 compliant token, such as `transfer`, `approve`, `transferFrom`, `balanceOf`, and `totalSupply`.

2. **ERC20Burnable:** The contract also inherits from `ERC20Burnable`, which adds the functionality to burn (destroy) tokens. The `burn` and `burnFrom` functions allow token holders (or approved addresses) to permanently remove tokens from circulation.

3. **Ownable:** Additionally, the contract extends `Ownable`, which is another OpenZeppelin contract. This means that the owner of the contract has special privileges, such as the ability to mint new tokens using the `mint` function. Only the owner can execute functions with the `onlyOwner` modifier.

**Functions:**

1. **constructor:** The constructor function is called once during the deployment of the contract. It sets the initial state of the token by providing a name ("MyToken") and a symbol ("JAYAXP") for the token.

2. **mint:** This function allows the owner (deployer) of the contract to create new tokens out of thin air and assign them to a specified address. The `mint` function takes two parameters: `to` (the address to which the tokens will be minted) and `amount` (the number of tokens to mint).

3. **Additional Functions:** Since this contract inherits from `ERC20`, it also inherits all the standard ERC-20 functions, such as `transfer`, `approve`, `transferFrom`, `balanceOf`, etc.

**Usage:**

To use this contract, you need to deploy it to the Ethereum blockchain using a development environment like Remix or Truffle. After deployment, the contract owner can call the `mint` function to create and distribute new tokens as needed.

**Note:** Before deploying or interacting with any smart contract on the Ethereum mainnet or any other live network, be sure to perform thorough testing and security audits to avoid potential vulnerabilities and risks.

**Disclaimer:**

This README file is for informational purposes only and does not constitute financial or investment advice. Use this contract at your own risk, and always exercise caution when dealing with smart contracts and digital assets.
