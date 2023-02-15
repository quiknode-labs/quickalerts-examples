## $BLUR Airdrop Claimed meets a certain threshold of tokens

### Description
Get a QuickAlert anytime a $BLUR airdrop is claimed and reaches a specific threshold of tokens.

### Blockchain & Network
All Blockchains and networks

### Expression Values
- `0x5283d291dbcf85356a21ba090e6db59121208b44` $BLUR ERC20 contract
- `0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef` Topic hash of ERC-20 Transfer event `Transfer (index_topic_1 address from, index_topic_2 address to, uint256 value)`
- `0x000000000000000000000000f2d15c0a89428c9251d71a0e29b39ff1e86bce25` BlurAirdrop Contract Address in 32 byte logs topic format (`from`)
- `50000` is the minimum amount of tokens claimed in order to fire the alert (`value`). This is value is adjustable.

### Expression
```
(tx_logs_address == '0x5283d291dbcf85356a21ba090e6db59121208b44') && (tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef') && (tx_logs_topic1 == '0x000000000000000000000000f2d15c0a89428c9251d71a0e29b39ff1e86bce25') && (tx_logs_data_int > 50000)
```

### Expected Result
```
[
  {
    "blockHash": "0xed3d98aca87800f283970caaa338145cca26607495fceb2d6ae03c7350d3037c",
    "blockNumber": "0xfdd7e5",
    "contractAddress": "",
    "cumulativeGasUsed": "0xaa0cac",
    "effectiveGasPrice": "0xa72ab9c12",
    "from": "0x9ee0711ca67dd00945e0090248c76a81347f3b1e",
    "gasUsed": "0x1b20d",
    "logs": [
      {
        "address": "0x5283d291dbcf85356a21ba090e6db59121208b44",
        "blockHash": "0xed3d98aca87800f283970caaa338145cca26607495fceb2d6ae03c7350d3037c",
        "blockNumber": "0xfdd7e5",
        "data": "0x00000000000000000000000000000000000000000000001273b5c1c58cea3db0",
        "logIndex": "0xfa",
        "removed": false,
        "topics": [
          "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
          "0x000000000000000000000000f2d15c0a89428c9251d71a0e29b39ff1e86bce25",
          "0x0000000000000000000000009ee0711ca67dd00945e0090248c76a81347f3b1e"
        ],
        "transactionHash": "0x9f6c5561dd9cc95ed49a9729cbfea3844139adfab29b91769c9df9b54a80eb0c",
        "transactionIndex": "0x77"
      }
    ]
  }
]
```
