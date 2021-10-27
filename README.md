# Candy-Machine-Mint


A candy machine is an on-chain Solana program (or smart contract) for managing fair mint. Fair mints:
* Start and finish at the same time for everyone.
* Won't accept your funds if they're out of NFTs to sell.

## Getting Set Up

### Prerequisites

* Ensure you have recent versions of both `node` and `yarn` installed.

* Follow the instructions [here](https://docs.solana.com/cli/install-solana-cli-tools) to install the Solana Command Line Toolkit.


### Installation

1. Fork the project, then clone down. Example:
```
git clone git@github.com:exiled-apes/candy-machine-mint.git
```

2. Build the project. Example:
```
cd candy-machine-mint
yarn install
yarn build
```

3. Define your environment variables using the instructions below, and start up the server with `npm start`.

#### Environment Variables

To run the project, first rename the `.env.example` file at the root directory to `.env` and update the following variables:

```
REACT_APP_CANDY_MACHINE_CONFIG=__PLACEHOLDER__
```

This is a Solana account address. You can get the value for this from the `.cache/temp` file. This file is created when you run the `metaplex upload` command in terminal.

```
REACT_APP_CANDY_MACHINE_ID=__PLACEHOLDER__
```

Same as above; this is a Solana account address. You can get the value for this from the `./cache/temp` file. This file is created when you run the `metaplex upload` command in terminal.

```
REACT_APP_TREASURY_ADDRESS=__PLACEHOLDER__
```

This the Solana address that receives the funds gathered during the minting process. More docs coming as we can test this.

```
REACT_APP_CANDY_START_DATE=__PLACEHOLDER__
```

This is a unix time stamp that configures when your mint will be open.

```
REACT_APP_SOLANA_NETWORK=devnet
```

This identifies the Solana network you want to connect to. Options are `devnet`, `testnet`, and `mainnet`.

```
REACT_APP_SOLANA_RPC_HOST=https://explorer-api.devnet.solana.com
```

This identifies the RPC server your web app will access the Solana network through.

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

