# AMM (Automated Market Maker)

This repository contains the implementation of an AMM (Automated Market Maker) contract in Solidity along with a front-end user interface that allows a user to connect and interact with the AMM contract.

## Getting Started

To get started with this project, follow these steps:

1. Clone this repository.
2. Install dependencies with `npm install`.
3. Run the local hardhat blockchain node with `npx hardhat node`.
4. Run the react client server with `npm start`.
5. Add the Hardhat network to a blockchain wallet such as MetaMask and connect to it.
6. Import the first 5 Hardhat accounts (Account #0, Account #1, Account #2, Account #3, Account #4) onto MetaMask (https://support.metamask.io/managing-my-wallet/accounts-and-addresses/how-to-import-an-account/#importing-using-a-private-key).
7. Deploy the contract to the local hardhat blockchain with `npx hardhat run scripts/deploy.js --network localhost.
8. Seed the AMM by running `npx hardhat run scripts/seed.js --network localhost`.
9. Connect to the website with any of the imported Hardhat accounts and interact with the AMM by swapping tokens, depositing liquidty, withdrawing shares and charting the price of tokens. Enjoy!

## Testing

To run the tests, use the following command: `npx hardhat test`

## Troubleshooting

If the application does not work, you can try the following troubleshooting steps:
- Clear activity and nonce data: Select the Hardhat network and Hardhat account on MetaMask that you are using to interact with the AMM, click the 3 vertical dots on the top right of the MetaMask extension, click "Settings", click "Advanced", Click "Clear activity tab data" and then Click "Clear". 
- Change the network from Hardhat to another network (like ETH Mainnet) and back to Hardhat on the MetaMask extension.
- Keep in mind that everytime the Hardhat node is restarted, you must run the deploy and seed scripts again and might have to repeat the above MetaMask specific steps for the application to perform appropriately.