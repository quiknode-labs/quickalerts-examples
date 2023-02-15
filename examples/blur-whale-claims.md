## $BLUR Airdrop Claimed meets a certain threshold of tokens

### Description
Get a QuickAlert anytime a $BLUR airdrop is claimed and reaches a specific threshold of tokens.

### Blockchain & Network
All Blockchains and networks

### Expression Values
- `0x5283d291dbcf85356a21ba090e6db59121208b44` $BLUR ERC20 contract
- `0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef` Topic hash of ERC-20 Transfer event `Transfer (index_topic_1 address from, index_topic_2 address to, uint256 value)`
- `0xF2d15C0A89428C9251d71A0E29b39FF1e86bce25` BlurAirdrop Contract (`from`)
- `50000` is the minimum amount of tokens claimed in order to fire the alert (`value`). This is value is adjustable.

### Expression
```
(tx_logs_address == '0x5283d291dbcf85356a21ba090e6db59121208b44') && (tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef') && (tx_logs_topic1 == '0xF2d15C0A89428C9251d71A0E29b39FF1e86bce25') && (tx_logs_data_int > 50000)
```

### Expected Result
TBD
