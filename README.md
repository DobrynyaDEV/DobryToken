# DobryToken (DTK)

ERC-20 token deployed on the **Ethereum Sepolia** testnet.
Built as part of a Vega blockchain course for MSU.

## Token details

| Parameter      | Value                                        |
|----------------|----------------------------------------------|
| Name           | DobryToken                                   |
| Symbol         | DTK                                          |
| Decimals       | 18                                           |
| Total supply   | 1,000 DTK (1,000 × 10¹⁸ base units)          |
| Standard       | ERC-20                                       |
| Network        | Ethereum Sepolia testnet                     |

## Deployment

| Item             | Link |
|------------------|------|
| Contract address | [`0x04B45A4DcFF7B625E88Dd38CE7ceBcb5C1963350`](https://sepolia.etherscan.io/address/0x04B45A4DcFF7B625E88Dd38CE7ceBcb5C1963350) |
| Deployment tx    | [`0xb6606fe8…aabfa5f91`](https://sepolia.etherscan.io/tx/0xb6606fe8a674db38b9b38e4beb6492d280f6f6ec8e546aca2307539aabfa5f91) |
| Token page       | [DobryToken on Etherscan](https://sepolia.etherscan.io/token/0x04b45a4dcff7b625e88dd38ce7cebcb5c1963350) |

## About decimals

ERC-20 tokens don't support fractions on-chain: all balances are stored as
integers in the smallest unit(with 18 decimals):

```
1 DTK      = 1,000,000,000,000,000,000 base units (10¹⁸)
1,000 DTK  = 10²¹ base units
```

## Contract

The token is implemented in [`DobryToken.sol`](./DobryToken/contracts/DobryToken.sol) and is based on
the [OpenZeppelin ERC-20](https://docs.openzeppelin.com/contracts/erc20)
implementation (MIT licensed).

## Tools

- [Remix IDE](https://remix.ethereum.org): writing, compiling and deploying
- [MetaMask](https://metamask.io): wallet and transaction signing
- [Sepolia Etherscan](https://sepolia.etherscan.io): verifying transactions

## How to interact

1. Add Sepolia to MetaMask browser extension/app and switch to it.
2. In MetaMask, choose **Import custom token** and paste the contract address.
3. Use `transfer(to, amount)` to send tokens. Remember that `amount` is in base
   units: to send 1 DTK, pass `1000000000000000000`.

## Disclaimer

This is a **testnet** token created for educational purposes! It has no
monetary value.

## License

MIT
