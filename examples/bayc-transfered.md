## Bored Ape Yacht Club (BAYC) Transfered

### Description
Get a QuickAlert anytime a transfer of a Bored Ape Yacht Club (BAYC) happens.

### Blockchain & Network
Ethereum Mainnet

### Expression Values
- `0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d` CryptoPunk Contract
- `0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef` Transfer Log

### Expression
```
(tx_logs_address == '0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d') && (tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef')
```

### Expected Result
```
{
  "block_number":15110668
  "topic":"raw-ethereum-mainnet"
  "chain":"ethereum-mainnet"
  "block":{
    "baseFeePerGas":"0x53509468e"
    "difficulty":"0x298709374aae57"
    "extraData":"0x6e616e6f706f6f6c2e6f7267"
    "gasLimit":"0x1c9c380"
    "gasUsed":"0x158d77d"
    "hash":"0x3b1e796cc7965348a2a8612515efe2ac7f33ba4e2d5c5dfbc10e78930d7946c3"
    "logsBloom":"0x1fae60ffde029a877e992cc8b9391bb76553bc76a07f87d79bff3d6ad6b2ed3ba6aff359dc6f61efca28919f39eff5275267fdbd3ba1bc7bbb9ac936f23ef7b478026d1415fd9ee8fcce66ceb6202765d9ed0f9ede77fb4ffa62fe799aedfe9c525a7eec633e7e76ed3f11c1f9fd3b7fef2ccd1fcaf89cd25f89fa3fa2087e61d6f1494e4efb79b63fefef692fd6522495399f79aded6798abf0b9e7fbb5b5a0ebf843b92f83657f7bf4eefb4d9c35fbeb1e58d3f5f7e9a6eb37efbf95fdff7fdbaeccc6258b02df5e2bbf3fbf96536d666df7f4b76a05345609ad6272fef8e31dbff97f68f6c70d3377f0f7f33e6a1033ee2232b16d8ef6d37f6eff7fd7f4fb"
    "miner":"0x52bc44d5378309ee2abf1539bf71de1b7d7be3b5"
    "mixHash":"0x26fb548d01a06d266787682c6adb2e4542db3916279b9ffd18bf0a3cfb0e8268"
    "nonce":"0x5d8a657e4d32696d"
    "number":"0xe6920c"
    "parentHash":"0x15bd4b0154013f2099848bd005e2e9bf845e94adf868fe8d1ce4e6897dadaca6"
    "receiptsRoot":"0xf15af584c9f955455fc4979f10a73e72352feb6f56ed0c730e76674b1617483b"
    "sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347"
    "size":"0x18c14"
    "stateRoot":"0x763a26fd9958a1e613d0b6a75133ce06d6645d7998b7182e7a16b7632327b251"
    "timestamp":"0x62c9eb1c"
    "totalDifficulty":"0xb5b78a5286b4ec893cc"
    "transactions": [...]
    "transactionsRoot":"0xdca0f3ed328aeedbb055947e5c6a849d7a38be653119659ec58e1aff7e232f3c"
    "uncles":[]
  }
  "receipts": [...]
}
```
