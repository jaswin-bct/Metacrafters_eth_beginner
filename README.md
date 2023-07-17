# Metacrafters_eth_beginner
#create a new token
Token:
This Solidity smart contract implements a basic token called "Meta Jas" (MJ). The contract allows for token minting and burning, while keeping track of token balances for different addresses.

Requirements
The contract is designed to fulfill the following requirements:

Token Details: The contract includes public variables to store information about the token, such as the token name, token abbreviation, and the total supply.

Address Balances: The contract uses a mapping (balance) to associate addresses with their respective token balances.

Mint Function: The contract provides a mint function that takes an address and a value as parameters. This function increases the total token supply by the given value and updates the balance of the sender's address accordingly.

Burn Function: The contract includes a burn function that works in the opposite way of the mint function. It takes an address and a value as parameters and deducts the value from the total token supply and the balance of the sender's address.

Safety Checks: The burn function incorporates conditionals to ensure that the balance of the sender's address is greater than or equal to the amount of tokens to be burned. If the balance is insufficient, an error message is returned.

Usage
Deploy the contract on the Ethereum network using Solidity version 0.8.18 or compatible.

Interact with the contract using the following functions:

mint(address _address, uint _supply): This function mints new tokens by increasing the total supply and the balance of the specified address. The _address parameter denotes the recipient's address, and _supply represents the amount of tokens to be minted.

burn(address _address, uint _supply): Use this function to burn tokens. The _address parameter identifies the sender's address, and _supply specifies the amount of tokens to be burned. The function deducts the tokens from the total supply and the balance of the sender's address. If the sender's balance is insufficient, an error message is returned.

License
This code is licensed under the MIT License. You can find the license text in the SPDX-License-Identifier comment at the beginning of the contract.

Note: Ensure that you are using a compatible Solidity compiler version (0.8.18) or newer to compile and interact with this contract.

