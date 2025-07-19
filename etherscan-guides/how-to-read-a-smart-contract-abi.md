# How to Read a Smart Contract ABI

Understanding a smart contract's ABI (Application Binary Interface) is essential when interacting with Ethereum contracts via tools like Etherscan, web3.js, or ethers.js. This guide breaks down what an ABI is, why it's important, and how to interpret it step by step.

---

## 🧠 What Is an ABI?

An **ABI** defines how to interact with a smart contract — the functions, inputs, outputs, events, and types it uses. Think of it as a *contract’s instruction manual*.

In Ethereum, ABIs are required to:

- Call functions on a deployed contract
- Decode events and transactions
- Connect front-end apps to the blockchain

---

## 🧩 Where to Find the ABI on Etherscan

1. Go to the smart contract’s Etherscan page (e.g., [Uniswap Router](https://etherscan.io/address/0xf164fC0Ec4E93095b804a4795bBe1e041497b92a#code)).
2. Scroll to the **Contract** section.
3. Click the **“Contract ABI”** tab to view or copy the ABI in JSON format.

---

## 🔍 How to Understand the ABI

Here's a simple example of an ABI snippet:

```json
[
  {
    "constant": true,
    "inputs": [],
    "name": "name",
    "outputs": [{ "name": "", "type": "string" }],
    "type": "function"
  }
]

---

### ✅ How to Upload This Guide to GitHub (Step-by-Step)

1. **Go to your repo**  
   → [https://github.com/Wjr10/web3-tech-writing-portfolio](https://github.com/Wjr10/web3-tech-writing-portfolio)

2. **Navigate to the `etherscan-guides` folder**  
   - Click on `etherscan-guides`

3. **Click “Add file” → “Create new file”**

4. **File name**:  
etherscan-guides/how-to-read-a-smart-contract-abi.md

5. **Paste the content** I gave you above into the editor.

6. Scroll down → Write a commit message:  
Add guide: How to Read a Smart Contract ABI

7. Click ✅ **“Commit new file”**

---

Let me know once it's uploaded — then we’ll update your `README.md` file with the new link and keep building your portfolio. 💪
