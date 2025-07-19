# How to Read a Smart Contract ABI

In Web3 development, the Application Binary Interface (ABI) is essential for interacting with smart contracts. An ABI defines the contract's functions, events, and how to encode/decode data when communicating with it from a frontend or script.

This guide explains what an ABI is, how to find one on [Etherscan](https://etherscan.io), and how to read and interpret its structure.

---

## 📌 What is an ABI?

An **ABI (Application Binary Interface)** is a JSON file that describes the interface of a smart contract — including its:

- **Functions** (e.g., `transfer`, `approve`)
- **Inputs/Outputs** for each function
- **Events**
- **Mutability** (e.g., `view`, `nonpayable`, `payable`)

ABIs allow Web3 libraries like **Web3.js**, **Ethers.js**, or **web3.py** to know *how* to communicate with the contract deployed on the blockchain.

---

## 🔍 How to Locate the ABI on Etherscan

To view a smart contract’s ABI:

1. Visit [https://etherscan.io](https://etherscan.io)
2. Enter the **contract address** in the search bar
3. Click the **"Contract"** tab
4. Scroll to the **"Code"** section
5. Locate the **"Contract ABI"** block — usually a long JSON array

![ABI section on Etherscan](https://raw.githubusercontent.com/Wjr10/web3-tech-writing-portfolio/main/assets/abi-location.png)

You can click the "Copy ABI to clipboard" button to use it in your code.

---

## 🧠 How to Read an ABI (Example Explained)

Here’s a simplified ABI snippet for a `transfer` function:

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
  "outputs": [],
  "stateMutability": "nonpayable",
  "type": "function"
}
