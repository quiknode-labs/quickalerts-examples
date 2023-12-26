## Bored Ape Yacht Club (BAYC) Transfered Improved Alert

### Description
Get a QuickAlert anytime a transfer of a Bored Ape Yacht Club (BAYC) happens with additional filtering and aggregation. Further refines results by filtering based on the BAYC contract address. Optimizes processing by handling blocks in batches of 1000.

### Blockchain & Network
Ethereum Mainnet

### Expression Values
- `0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d` BAYC Contract
- `0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef` Transfer Log

### Expression
```
(tx_logs_address == '0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d') && (tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef')
```

### Expected Result
```
[
  {
  "blockchain": "Ethereum Mainnet",
  "description": "Bored Ape Yacht Club (BAYC) Transferred",
  "expression": "(tx_status == 1) && (tx_logs_address == '0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d') && (tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef')",
  "aggregation": {
    "type": "block_range",
    "value": 1000
  },
  "filters": {
    "contract_address": "0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d"
  }
}

]
```
