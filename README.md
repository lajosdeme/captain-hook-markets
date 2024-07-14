# Captain Hook Markets
![image](https://github.com/user-attachments/assets/98a27aa1-310c-42fb-854b-d14a533805b7)

Cross-chain perps market using Pancake Swap V4 pools and hooks. Using ERC20 tokens wrapped in OFTs as pool assets and for cross-chain financing.

Captain Hook Finance is a perpetual futures market that interacts with Pancake Swap V4 Pools. It is permissionless, oracle-free, and cross-chain.

Captain Hook Finance relies heavily on Pancake Swap V4 Pools as well as LayerZero OFTs. We allow users to trade options on any V4 Pool that is created in Pancake Swap V4.

Further than that, we add significant cross-chain capabilities. Our token "OFTWrappedERC20" allows any ERC20 token to be wrapped into an OFT. This token exposes a new function "sendAswCollateral", that allows the token to be deposited as collateral cross-chain on a Captain Hook Finance market. We achieve this by modifying the default "send" function on the OFT, adding our own custom logic to it.

The implementation of the perps market is inspired by [Hook Finance](https://github.com/hook-finance/hook-finance-hook).

## Deployed contract addresses:

Optimism Sepolia:
- (fake) USDC: 0xcE1Fd4B4CD044dfc4b488633A4BEBd9AB61E116a
- Amazing Token (AT): 0xFc5cea8407Be982eCfA64041cFfe85A69f32c0B2 (random ERC20 for the pool)
- OFT Wrapped USDC: 0xAd6cD4472D30911e660BD19024fD36Ef5f126e89
- OFT Wrapped AT: 0x105fd7E5A68A5ab2545e49Da021F94cb73D042b8

Base Sepolia:
- Captain Hook: 0xD9f64CA93CDB3c5F7DE29E975b0dBE9e2446F6Aa
- Vault: 0x5099c42484665CD0fd12Fc2EEBFeF2dC20948F1b
- CLPoolManager: 0x6ff773dAD3B7f16c528A2d55fA3Fe460e78A0Def
- 
- wUSDC: 0xAdFCbF60d5C5b8739B458602Aa64f7313c0D9FF1 (pair OFT for the OP one)
- wAT: 0xBD913298f2E2170a87B75Dc851fa9Fa5394dF48A (pair OFT for the OP one)
