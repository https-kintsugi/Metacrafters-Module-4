# DegenToken Smart Contract

DegenToken is an Ethereum smart contract built using Solidity. It extends the OpenZeppelin ERC20 and Ownable contracts to create a custom ERC20 token with additional features, including a simple inventory system where users can buy items from a merchant.

## Features

- Custom ERC20 token named "Degen" with the symbol "DGN".
- Minting new tokens can only be done by the contract owner.
- Burning tokens allows a user to decrease their own balance.
- Transferring tokens includes basic validation checks.
- Users can buy items from a merchant using their token balance, with the inventory being tracked on-chain.


## Contract Deployment

You can deploy this contract to an Ethereum network using Truffle, Hardhat, or other Ethereum development tools. Make sure to configure the deployment parameters.

## Contract Interaction

### Mint Tokens

The mint function allows the contract owner to create and send new tokens to a specified address.

### Burn Tokens

The burn function allows a user to burn a specified amount of their own tokens.

### Transfer Tokens

The transfer function overrides the default ERC20 transfer behavior to include basic validation checks.

### Buy Items from Merchant

The buyFromMerchant function allows a user to buy an item from the merchant. The function checks if the user has sufficient balance and updates their inventory on a successful purchase.

### Inventory Item Count

The InventoryItemCount function returns the total number of items available in the merchant's inventory.