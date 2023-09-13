# Decentralized NFT Marketplace

This is an open decentralized NFT Marketplace built with smart contracts powered by Ethereum. It provides a platform for users to mint their own NFTs and list them on a marketplace for trading and showcasing their digital assets.

## Getting Started

These instructions will help you set up a local development environment for this project.

### Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine
- [Git](https://git-scm.com/) for cloning the repository
- [Metamask](https://metamask.io/) wallet with a Ganache testnet network configured

### Installation

1. Clone the repository:

    ```shell
    git clone https://github.com/ashutosh0111/NFTMarketplace.git
    ```

2. Navigate to the project directory:

    ```shell
    cd NFTMarketplace
    ```

3. Install project dependencies:

    ```shell
    npm install
    ```

4. Add your Ethereum account private key to the project. Create a `.env` file in the project root directory and add the following:

    ```env
    PRIVATE_KEY="enter your private key"
    ```

5. Add a Ganache network to your Metamask wallet with the name `ganachetestnet`.

6. Deploy the smart contracts to the Ganache testnet:

    ```shell
    npx hardhat deploy
    npx hardhat run --network ganachetestnet scripts/deploy.js
    ```

7. Create a Pinata Cloud account and obtain your private API key and secret key.

8. Add the Pinata API keys to your `.env` file:

    ```env
    REACT_APP_PINATA_KEY="your pinata app key"
    REACT_APP_PINATA_SECRET="your pinata secret key"
    ```

### Running the Application

Start the NFT Marketplace application:

```shell
npm start
```

Now you can access the application locally at [http://localhost:3000](http://localhost:3000) and begin minting and trading NFTs.

## Technologies Used

- Solidity
- React.js
- Hardhat
- ethers.js
- Ganache
- Metamask
- IPFS
