
# ERC20 Token Contract


The code you provided is an implementation of an ERC20 token contract in Solidity. Here's a brief description of the contract and its functionalities:

## Description

The ERC20 token contract provides a standardized implementation for managing fungible tokens. This contract includes the essential ERC20 functionalities such as tracking the total supply of tokens (totalSupply), individual account balances (balanceOf), and allowances for delegated transfers (allowance). It supports key operations such as transferring tokens (transfer), approving third parties to spend tokens (approve), and transferring tokens on behalf of an owner (transferFrom). Additionally, the contract includes mechanisms for minting new tokens (mint) and burning existing tokens (burn), allowing for the creation and destruction of tokens as needed.

Beyond the standard ERC20 features, this contract integrates an in-game currency system and item management. It maintains a variable playerCurrency to manage the player's in-game currency and provides a mapping (itemPrices) for storing item prices. The purchaseItem function allows players to spend their in-game currency to acquire items, and the purchaseCurrency function enables adding more currency to the player's balance.

## Getting Started
 
 ### Installing code

 You can clone this repo or download zip file and run it locally or you can run the code on remix 

 Head over to this website: https://remix.ethereum.org/.
 ### Executing the code

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., ERC20game.sol). Copy and paste the solidity file into the remix file

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.17" (or above version), and then click on the "Compile ERC20game.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "solidity" contract from the dropdown menu, change the environment to 'Injected provider' and connect your metamask account, and then click on the "Deploy" button.

### Subnet 
 
Follow the below github repository's readme file in order to install avalanche CLI to your Ubuntu or Mac terminal:
 
 [https://docs.avax.network/tooling/cli-guides/install-avalanche-cli](https://github.com/ava-labs/avalanche-cli)

In order to create a subnet, we run -

```
avalanche subnet create mySubnet
```

In order to deploy the created subnet, we run -

```
avalanche subnet deploy mySubnet
```

To connect your subnet to metamask, you will need to :

* Add network manually and enter Name, RPC URL, Token Symbol and Chain ID that you entered while creating the subnet.
* Import account with test tokens by entering the private key that you get from the terminal after you deploy the subnet.

 
## License

This code is licensed under the [MIT](https://choosealicense.com/licenses/mit/) license.See the LICENSE file for more information.


