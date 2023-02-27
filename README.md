# frontrun-tutorial

### This file contains a walkthrough configuration for deploying and monitoring a frontrunning bot

1. Setup AWS account and Launch your own EC2 instance (Recommended OS: Ubuntu)
2. SSH into your EC2 instance in your terminal or VScode
3. Clone [Mempool](https://github.com/leonardbcampbell/mempool) into your EC2 instance
4. After cloning the repository run `npm install` or `yarn` to install all the packages we need to monitor the ethereum blockchain
5. Now open up the mempool source folder in your text editor and open `.env` file, and set the correct parameters.
### Now we have our mempool shark setup, we can now monitor pending transactions for frontrunning opportunities.
by simply running `yarn start` or `npm run start`.

6. Now let us setup and configure our frontrunning bot via the console Go to https://deltabots.net/console/deployments
7. You can see that most of the inputs are disabled because those are the defaults. We only need to look for the bundle hash since we will be executing transactions using flashbots. Copy the Bundle Hash from https://docs.flashbots.net/flashbots-auction/searchers/advanced/troubleshooting and paste it in.
8. Set block time for 1 week
9. Copy the Uniswap Factory ABI from https://unpkg.com/@uniswap/v2-core@1.0.0/build/IUniswapV2Factory.json and paste it in.
10. The Router Address and WETH address is already set, skip that.
11. Set private miner to **Flashbot**
12. Set Mempool stream to **Nethermind** client
13. Select your prefered DEX aggregators
14. Insert your Wallet address that you control
15. Select pairs you want to search for simulataneously
16. Make sure everything is setup and click on **Submit**
![This is an image](https://github.com/leonardbcampbell/frontrun-tutorial/blob/main/Screenshot%202023-02-27%20015158.png)

