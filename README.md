# frontrun-tutorial

### This file contains a walkthrough configuration for deploying and monitoring a frontrunning bot

1. Setup AWS account and Launch your own EC2 instance (Recommended OS: Ubuntu)
2. SSH into your EC2 instance in your terminal or VScode
3. Clone [Mempool](https://github.com/leonardbcampbell/mempool) into your EC2 instance
4. After cloning the repository run `npm install` or `yarn` to install all the packages we need to monitor the ethereum blockchain
5. Now open up the mempool source folder in your text editor and open `.env` file, and set the correct parameters.
### Now we have our mempool shark setup, we can now monitor pending transactions for frontrunning opportunities.
by simply running `yarn start` or `npm run start`.

