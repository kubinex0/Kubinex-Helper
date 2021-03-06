# kubinex-Helper
This package acts as a single source of truth for helper contracts used by the [kubinex](http://kubinex.finance/).

## Install
```
npm i kubinex-helper
```
## Reference
### 1. BEP20Helper
```javascript
//Function
//Transfers out BEP20 tokens to ReceiverAddress
TransferToken(TokenAddress, ReceiverAddress, Amount)

//Function
//Checks balance of BEP20 tokens
CheckBalance(TokenAddress, WalletAddress)

//Function
//Transfers in BEP20 Tokens from AddressToTransferFrom(approval required). 
TransferInToken(TokenAddress, AddressToTransferFrom, Amount)
```
### 2. ETHHelper
```javascript
//function
//transfers ETH to ReceiverAddress
TransferETH(ReceiverAddress, Amount)
```
### 3. GovManager
```javascript
//modifier
//allows functions to be called by the gov contract
onlyOwnerOrGov

//function
//sets the address of Gov contract
setGovernerContract(address)
```
### 4. Token
BEP20 Token used for Testing Purpose

### 5. IWhiteList
Interface to interact with WhiteList Contract
