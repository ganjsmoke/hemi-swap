
# Auto Daily Swap Hemi

This project is an automated bot that swaps tokens on the Hemi network every 6 hours support multiple wallets. It allows users to perform token swaps automatically at regular intervals, without manual intervention.

Register : https://points.absinthe.network/hemi/start
Invite Code : c7e7f4a9

## Features
- **Automatic Token Swap**: Performs token swaps using a specified contract on the Hemi network.
- **Multi-Wallet Support**: The bot reads private keys from a file and performs the swap on multiple wallets.
- **Custom Transaction Count**: You can specify how many transactions to execute per wallet.
- **Auto-Recovery on Failure**: The bot will retry failed transactions up to a specified limit with a delay between attempts.
- **Recurrent Swaps**: The bot is set to perform swaps every 6 hours automatically.

## Requirements

- **Node.js**: Ensure you have [Node.js](https://nodejs.org/en/) installed.
- **Private Keys**: You must provide a `private_keys.txt` file with your wallet private keys (one per line).
- **Hemi Network Testnet**: The bot is configured to use the Hemi testnet. Ensure you have testnet tokens to perform swaps.

## Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ganjsmoke/hemi-swap.git
   cd hemi-swap
   ```

2. **Install dependencies**:
   This project uses `web3` and `chalk`. Install the required dependencies using npm:
   ```bash
   npm install
   ```

3. **Configure the private keys**:
   - Create a file named `private_keys.txt` in the root directory of the project.
   - Paste your wallet private keys, each on a new line. Example:
     ```
     0xPRIVATE_KEY_1
     0xPRIVATE_KEY_2
     ```

4. **Run the bot**:
   - To start the bot and perform the initial set of transactions, simply run:
     ```bash
     node index.js
     ```
   - The bot will prompt you to enter the number of transactions you want to perform per wallet. It will use this value for subsequent executions.

5. **Auto Execution**:
   - The bot will automatically perform token swaps every 6 hours.
   - On each execution, it will not ask for the number of transactions again. The value will be used from the first prompt.


## Disclaimer

This bot is intended for use on the Hemi Testnet. Be cautious when using real tokens, and always test on the testnet first. Never share your private keys with anyone.

## Contact

For any issues or inquiries, you can contact me via [Telegram](https://t.me/airdropwithmeh).

---

**Bot created by**: [Telegram - @airdropwithmeh](https://t.me/airdropwithmeh)
