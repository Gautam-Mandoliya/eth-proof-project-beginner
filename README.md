# eth-proof-project-beginner

# MyCoin Contract

This contract implements a basic cryptocurrency token called MyCoin. It allows users to mint (create) and burn (destroy) tokens, as well as retrieve token balances.

# Requirements

1. The contract should have public variables to store the details of the coin, including the token name, token abbreviation, and total supply.
2. It should have a mapping of addresses to token balances.
3. The contract should include a mint function that increases the total supply by a given value and increases the balance of the sender's address by the same amount.
4. A burn function should be implemented to decrease the total supply and deduct the specified value from the sender's balance.
5. The burn function should include conditionals to ensure that the sender's balance is greater than or equal to the amount being burned.
   
#Installation

No installation is required for this contract. It can be deployed and interacted with directly on a supported Ethereum network.

Usage
To use the MyCoin contract, follow these steps:

1. Deploy the contract on an Ethereum network of your choice.
2. Set the token name and abbreviation by providing the respective values in the constructor.
3. Interact with the contract's functions using a smart contract or a web3-enabled application.
   
 # Mint Function

The mint function allows the creation of new tokens. It takes two parameters: an address and a value. 
The function increases the total supply by the given value and updates the balance of the sender's address accordingly.

Example usage:
MyCoin myCoin = new MyCoin("MyCoin", "MYC");
myCoin.mint(msg.sender, 100); // Mint 100 MyCoins for the sender

Retrieving Balances
The balances mapping allows you to retrieve the token balance of an address.

Example usage:

MyCoin myCoin = new MyCoin("MyCoin", "MYC");
myCoin.mint(msg.sender, 1000); // Mint 1000 MyCoins for the sender

// Retrieve the balance of a specific address
uint256 balance = myCoin.balances(msg.sender);

# License

This project is licensed under the MIT License. See the LICENSE file for more information.
