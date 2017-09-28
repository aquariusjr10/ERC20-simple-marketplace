# Simple Marketplace

A simple contract to "safely" sell/buy ERC20 tokens made while learning solidity.

# Usage

The seller creates a trade contract form the marketplace, inserting the token address, the amount to sell and the price (in wei). Once the contract is created the seller must approve it as a token spender (ERC20 approve())

The buyer sends ether to the trade contract, tokens are sent immediately. The seller can now withdraw his earnings, destroying the contract.

# In case of trouble

If the seller sends the tokens to the trade contract, there is a function to recover them, but the marketplace owner must be trusted to do so.