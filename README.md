# core-pyth-feed-boilerplate

Pyth Feed Boilerplate is a React-based dApp for fetching and displaying real-time price feeds from the Pyth Network. This boilerplate provides a quickstart template for developers to quickly create similar applications on the Core blockchain.

Purpose: The quickstart guide helps developers rapidly set up a functional dApp with essential setup instructions and code snippets. For detailed instructions and advanced configurations, refer to the full-length guide further down.

## Quickstart

Project Setup: Clone the repository and install dependencies.
Configuration: Set up the Pyth price feed smart contract and integrate it with the React app.
Running the Application: Start the app and view real-time price feeds.

### Prerequisites

Before setting up the project, ensure you have the following installed:

- [Node.js and npm](https://nodejs.org/en/download/)
- [MetaMask](https://metamask.io/download.html) browser extension
- [Git](https://git-scm.com/downloads)

### Setup

### 1. Clone the Repository

Clone the repository to your local machine using GitHub Desktop or Git:

```zsh
git clone https://github.com/your-username/pyth-feed-boilerplate.git
cd pyth-feed-boilerplate
```

### 2. Install Dependencies
Navigate to the project directory and install the necessary dependencies:

```
npm install
```
### 3. Configure the Project

- Add **Private Key**: Create a '**secret.json**' file in the project root and add your private key.

```json
{
  "PrivateKey": "your-private-key-here"
}
```
>Once deployed, update Smart Contract Address: Open src/App.js and replace 0xYourContractAddress with your deployed contract address on the Core blockchain.

### 4. Install Babel Plugin
Install the Babel plugin to avoid dependency issues:

```zsh
npm install --save-dev @babel/plugin-proposal-private-property-in-object
```

### 5. Run the Application
Start the React application:

```zsh
npm start
```

### 6. Access the Application
Open your browser and navigate to if it has not already:

```arduino
http://localhost:3000
```
### Troubleshooting
Error: One of your dependencies, babel-preset-react-app, is importing the "@babel/plugin-proposal-private-property-in-object" package without declaring it in its dependencies.
Solution: Install the Babel plugin manually:

```zsh
npm install --save-dev @babel/plugin-proposal-private-property-in-object
```

**Error**: MetaMask - RPC Error: Request of type 'wallet_requestPermissions' already pending.

**Solution**: Open MetaMask and approve or reject the pending permission request.

**Error**: no matching function (argument="name", value="updatePrice", code=INVALID_ARGUMENT, version=abi/5.7.0)

**Solution**: Ensure the ABI file is up-to-date and contains the correct function names.
