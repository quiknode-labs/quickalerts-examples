## New Ether Balance Alert

### Description
Get a QuickAlert anytime there is a change in the Ether balance of a specific address.

### Blockchain & Network
All Ethereum-based Blockchains and networks

### Expression Values
- `0x742d35Cc6634C0532925a3b844Bc454e4438f44e` is the target Ethereum address

### Expression
```
(tx_logs_address == '0x742d35Cc6634C0532925a3b844Bc454e4438f44e')
```

### Expected Result

```
{
  "block_number": 12345678,
  "topic": "raw-ethereum-mainnet",
  "chain": "ethereum-mainnet",
  "block": {
    "baseFeePerGas": "0x2f0d6189d",
    "difficulty": "0x29e5912853b0df",
    "extraData": "0x466c6578706f6f6c2f53322f484b202d204672616e6b66757274",
    "gasLimit": "0x1c9c380",
    "gasUsed": "0x1c97e3b",
    "hash": "0xcb7610794ffa5eab044e3ce4330cb0551ef71c1548bbb6e54a9f3276529c1dea",
    "logsBloom": "0xdf77d1af6388bf8ef7a8fefba855dffbaab34d389d1527faf399e56b3f22edfdfd7ddfffbd6beefc4cb6dfeb615dcfc7ff8ba5657b97fcd1fff7dee77fbef3793e6a4aa8bd1febefebf2f6d946dffdab74ddebf7ed7eb7c37e7e3fddaefadb119e79b8f6fa23efce2fe631a7beabc9fde7f2df700e4f77ecbbf5bdda9afdaf7679fe876edbbe7f7fdfdf635ddb67db175e163cddc3fdd6bff7afdde7ffb9dde7fbfd75bbb4eb7c2efadb4dc39fdfcfe30fdfcee2f8fd293ebdffbefffd7b9ee7fd18ecbbbfd260fe1bdf4faa9dfede96f7fd7fd2df6b23bfd71779ff53df3c3fdeb5ed5f7dc8effab386b6ef57bc5efedde268bb6dec95fda4fafb9bda3ff0ab",
    "miner": "0x7f101fe45e6649a6fb8f3f8b43ed03d353f2b90c",
    "mixHash": "0x645f30204950025047c6ad5104ffc219f5dff2aa5a76ea1fe3c79dedb5639158",
    "nonce": "0x9ecc58b527c0147c",
    "number": "0xe768f3",
    "parentHash": "0x11251096da1ae5bd0006293a335ba29b262e6cfa12a5ecbb90ca63098c60a6d3",
    "receiptsRoot": "0xdcdb718d91fd20059bafb1b96581f4f15cae73dbd1bd87f62853e3a18c5a5f4c",
    "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
    "size": "0x26555",
    "stateRoot": "0x77a88e9cdb669c8d822c5f4e2b2229d4e7e37cb7aeab0d5624aaa77f76633542",
    "timestamp": "0x62d51fb4",
    "totalDifficulty": "0xb7e1df721c65695f759",
    "transactions": [
      // Details of individual transactions in the block
    ],
    "transactionsRoot": "0x8fd9679239e1a99e7f2f9fd08c892cc7a721dc9ee6343b53258bae44349d192e",
    "uncles": []
  },
  "receipts": [...]
}

```