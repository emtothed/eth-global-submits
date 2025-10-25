## Usage :
1. run `forge soldeer install` to get contract dependencies.
2. run `cd node-scripts && npm i` to get node modules.
3. edit `./.env.example` and add your private keys and rename it to `.env`
4. edit `./node-scripts/src/constants.ts.example` and add you private keys and addresses and rename it to `constants.ts`
5. run anvil on your device
6. run command below to deploy the contract on the anvil
```
source .env && forge script script/DeployUniversalSwapper.s.sol --rpc-url $RPC_URL --private-key $PRIVATE_KEY --broadcast
 ```
1. run `tsx|ts-node node-scripts/src/universal-swap.ts` to performe a swap from USDC to WETH

## notes:
1. your account must have enough funds before swap
2. addresses are for ethereum mainnet and forked chain should fork mainnet too.