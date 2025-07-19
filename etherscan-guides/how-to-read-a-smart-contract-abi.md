# How to Read a Smart Contract ABI

Smart contracts are the building blocks of decentralized applications (dApps). To interact with these contracts, especially via scripts or Web3 frontends, we use something called the **ABI** — Application Binary Interface.

## 🧠 What is an ABI?

The **ABI** is essentially a description of how to interact with a smart contract on Ethereum. It defines:
- The **functions** a contract exposes (e.g., `transfer`, `balanceOf`)
- The **parameters** these functions accept
- The **outputs** they return
- Whether the function changes the blockchain state or is read-only

If you think of the smart contract as a machine, the ABI is the manual.

## 🔍 Where to Find the ABI on Etherscan

Let’s say we want to inspect the ABI of a deployed contract, such as a popular ERC-20 token.

1. Go to [https://etherscan.io](https://etherscan.io).
2. Paste the contract address into the search bar.
3. Navigate to the **Contract** tab.
4. Scroll down to the **Contract ABI** section.

![ABI Location on Etherscan](https://raw.githubusercontent.com/Wjr10/web3-tech-writing-portfolio/main/assets/abi-location.png)

Click **"Copy"** to save the entire ABI to your clipboard for use in your dApp, script, or Web3 library.

## 🧩 Understanding the ABI Structure

Here’s a short sample from a contract ABI:

```json
[
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
]
