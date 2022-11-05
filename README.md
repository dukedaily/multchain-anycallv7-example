 This repo would deploy a solidity contract on two chains and send a text message from chain A to chain B.
 This is purposed to showcase anyCall V7 cross-chain messaging capability. 
 
0. Set up the environments with yarn or npm
yarn || npm install

 1. add prvkey in .env.example file and add etherscan apis if you want to auto verify. Change the .env.example filename to .env

 2. Deploy the example contract on ftm testnet and bnb testnet. Make sure you have gas tokens on both chains.
 Run these two commands:

 ```sh
 # 0x48636063bD54f705E8c5b5858a0462F896c05ADC
yarn hardhat deploy --network ftmtest

# 0x8B43B8E728Af345830732A6A0Bd78BB754Fd51a3
yarn hardhat deploy --network bnbtest
 yarn hardhat run ./scripts/1testanycall.js --network bnbtest
 ```