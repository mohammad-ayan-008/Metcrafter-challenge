# Solidity Vault and ERC20 Contract
This repository contains two Solidity contracts: Vault and ERC20. The Vault contract provides functionality for depositing and withdrawing ERC20 tokens while minting and burning shares representing ownership within the vault. The ERC20 contract is a basic implementation of the ERC20 token standard.

# Contracts
## Vault
The Vault contract manages deposits and withdrawals of ERC20 tokens. It allows users to deposit tokens, minting shares equivalent to the deposited amount, and withdraw tokens by burning shares. Below are the key functions of the Vault contract:

deposit(uint _amount): Allows users to deposit ERC20 tokens into the vault, minting shares for the sender.
withdraw(uint _shares): Allows users to withdraw ERC20 tokens from the vault by burning shares.
## ERC20
The ERC20 contract is a basic implementation of the ERC20 token standard. It provides functionalities for transferring tokens, approving token transfers, and allowance management. Below are the key functions of the ERC20 contract:

transfer(address recipient, uint amount): Transfers tokens from the sender's account to the recipient.
approve(address spender, uint amount): Approves the spender to spend a specified amount of tokens on behalf of the sender.
transferFrom(address sender, address recipient, uint amount): Transfers tokens from one account to another if approved by the sender.
mint(uint amount): Mints new tokens and adds them to the sender's account.
burn(uint amount): Burns a specified amount of tokens from the sender's account.
Interacting with Remix
To interact with the contracts using Remix, follow these steps:

1. Open Remix IDE (https://remix.ethereum.org/).
2. Create new files for each contract: Vault.sol and ERC20.sol.
3. Copy the respective contract code into each file.
4. Compile the contracts by selecting the appropriate compiler version.
5. Deploy the ERC20 contract by providing initial parameters (if required).
6. Deploy the Vault contract, passing the address of the deployed ERC20 contract as a constructor argument.
7. Interact with the contracts using Remix's interface for calling functions and transactions.
8. Ensure you have a suitable environment configured in Remix (e.g., injected Web3 for testnets or a local blockchain) to deploy and interact with the contracts.
