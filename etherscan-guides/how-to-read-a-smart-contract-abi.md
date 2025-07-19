# How to Read a Smart Contract ABI

The Application Binary Interface (ABI) defines how to interact with a smart contract on the Ethereum blockchain. It acts as the bridge between the contract and external applications.

## Why ABI Matters

Smart contracts are compiled into bytecode, which is unreadable by humans. The ABI provides a human-readable interface that outlines:

- Functions available in the contract
- Function names and inputs/outputs
- Events emitted
- Variable types

## Where to Find an ABI

To find a contract's ABI on Etherscan:

1. Search for the contract address on [Etherscan.io](https://etherscan.io/).
2. Scroll to the **Contract** tab.
3. Under **Contract ABI**, click the **Copy** icon.

> 🔍 Tip: If the contract is verified, the ABI will be publicly available.

## How to Read the ABI Structure

An ABI is a JSON array of function and event descriptors. Here's an example of a `transfer` function in an ABI:

```json
{
  "inputs": [
    {
      "internalType": "address",
      "name": "recipient",
      "type": "address"
    },
    {
      "internalType": "uint256",
      "name": "amount",
      "type": "uint256"
    }
  ],
  "name": "transfer",
  "outputs": [
    {
      "internalType": "bool",
      "name": "",
      "type": "bool"
    }
  ],
  "stateMutability": "nonpayable",
  "type": "function"
}
