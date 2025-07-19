# How to Fetch Ethereum Wallet Balance Using Etherscan API

This beginner-friendly guide will walk you through how to fetch the ETH balance of any Ethereum wallet using the Etherscan API.

## 🛠️ Prerequisites

- A free Etherscan API key (get one at [etherscan.io](https://etherscan.io/myapikey))
- A valid Ethereum wallet address
- A code editor or API testing tool (e.g., Postman, Insomnia, or your browser)

---

## 🔗 Step 1: Understand the API Endpoint

To check the ETH balance of a wallet, use this Etherscan API endpoint:

https://api.etherscan.io/api

You’ll be sending a GET request with the following parameters:

| Parameter   | Value                     | Description                       |
|-------------|---------------------------|-----------------------------------|
| `module`    | `account`                 | Specifies the account module      |
| `action`    | `balance`                 | Fetches the balance               |
| `address`   | `<wallet_address>`        | Replace with the actual address   |
| `tag`       | `latest`                  | Gets the latest balance snapshot  |
| `apikey`    | `<YourApiKeyToken>`       | Your personal Etherscan API key   |

---

## 🧪 Step 2: Sample API Request

```bash
Replace:

    0xde0B295... with the actual wallet address

    YourApiKeyToken with your real API key
curl "https://api.etherscan.io/api?module=account&action=balance&address=0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe&tag=latest&apikey=YourApiKeyToken"
{
  "status": "1",
  "message": "OK",
  "result": "40807285323500000000"
}
40807285323500000000 wei = 40.8072853235 ETH

---

### ✅ What’s Next?

Now go to your GitHub repo and follow the **exact upload steps** we discussed previously to:

- Create the file at:


