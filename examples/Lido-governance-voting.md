## Governance-votecast-alert

### Description
Tracking Vote propsals of Lido Governance token Contract

### Blockchain & Network
Ethereum-Mainnet

### Expression Values
- `0x5a98fcbea516cf06857215779fd812ca3bef1b32` LDO contract address
- `0x853654a704a354a654a354a354a354a354a354a354a354a354a354a354a354a3` Event hash for proposal created/VoteCast/Proposal Executed

### Expression
```
(tx_logs_address == '0x5a98fcbea516cf06857215779fd812ca3bef1b32') && (tx_logs_topic0 == '0x654a54a354a354a354a354a354a354a354a354a354a354a354a354a354a354a3')
```

### Expected Result

```
{
"block_number":18875771
"topic":"raw-ethereum-mainnet"
"chain":"ethereum-mainnet"
"block":{
"baseFeePerGas":"0x40ca0d04c"
"difficulty":"0x0"
"extraData":"0x546974616e2028746974616e6275696c6465722e78797a29"
"gasLimit":"0x1c95111"
"gasUsed":"0x100333f"
"hash":"0x4f2f2dc30655a6bb553766c610b27fcebe5d7a6836b931d0c6eff03cd18f4124"
"logsBloom":"0x10edc14743a81edc554d368a9c436b2c94d1e0a04a0632255a694d1f7cc654bae87f31a5e85a0a84aafdbbcb9112dffcd3c3a81bab1bbdc9de7511f948f82ae654ea753aeb5b28bfca8a6e39f02b796b95dc028f4fe6090a3d6e9c4d843faad49f4c0fa00a428a3fa3cd7d4968286c77c9344baf71420f48570be1d920890e372500d7d5da358659c1cf95a7e7a2c8e2ad1187a5abfa8ec9d42d20ca4eb55c79feee2060fa822b8206f168ee990536a664b1c7d940a3a8da21eb25b246da29693c619623305208e29f60700f1843d81208fd3f071123b65e27c833271876edc4b03ca56de891446eda4594a6e221fcc4aa4e7b5ad8cf9b4064893dbeb68614be"
"miner":"0x4838b106fce9647bdf1e7877bf73ce8b0bad5f97"
"mixHash":"0x5d851fb40a1f719df79297425776acf2fe6cfa2e75e5097ecdbde73fe46f31ea"
"nonce":"0x0000000000000000"
"number":"0x120057b"
"parentHash":"0x95d703169d61617f613226a4a336c26a80bc8b23cf85d38066b9a93b2846b2f9"
"receiptsRoot":"0x0d73fffbde691b2a93d3a83f40e0ec4ad9cae0bd9a74bfc407ab07a9d77c7a1a"
"sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347"
"size":"0x3dcc2"
"stateRoot":"0xf94bd2c0aeae85378f38634a03edd69a07b756dd3fb22091f300ce51ba5b351d"
"timestamp":"0x658bde3b"
"totalDifficulty":"0xc70d815d562d3cfa955"
"transactions":
[0 - 100]
[100 - 181]
"transactionsRoot":"0xa7557a01b16fa16bb7f2ae96bd3afec22e87a1625ae552f48e2394f6b18ddc07"
"uncles":[]
"withdrawals":[...]
"withdrawalsRoot":"0x8cfafe1cdf692ad2db2216bc37622247f84c91f110babc665e69848aeebf4b95"
}
"receipts":
[0 - 100]
[100 - 181]
}
```