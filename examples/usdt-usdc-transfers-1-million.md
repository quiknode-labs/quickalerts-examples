## USDT and USDC transfers with at least 1 million

### Description

Get a QuickAlert when at least 1 million USDT or USDC is transferred.

This QuickAlert listens to the `Transfer` event of USDT and USDC.

Here's the event definition, `Transfer (index_topic_1 address from, index_topic_2 address to, uint256 value)`.

### Blockchain & Network

Ethereum Mainnet.

> **Note:** To support other EVM-compatible network, change the `tx_logs_address` to the **contract address** of USDT and USDC on that specific network.
>
> Also make sure to change the `tx_logs_data_int` to reflect the **number of decimals** in the USDT and USDC contract.

### Expression Values

- `0xdac17f958d2ee523a2206206994597c13d831ec7` contract address of **USDT** on **Ethereum Mainnet**
- `0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48` contract address of **USDC** on **Ethereum Mainnet**
- `0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef` Topic hash of **Transfer** event
- `^0x[0]{24}[a-fA-F0-9]{40}$` regex to validate wallet addresses.
- `''` to make sure tx_logs_topic3 is empty
- `1000000000000` at least **1 million**, including **6 decimals** for USDT and USDC

### Expression

```
(
  tx_logs_address == '0xdac17f958d2ee523a2206206994597c13d831ec7' ||
  tx_logs_address == '0xa0b86991c6218b36c1d19d4a2e9eb0ce3606eb48'
) &&
tx_logs_topic0 == '0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef' &&
tx_logs_topic1 =~ '^0x[0]{24}[a-fa-f0-9]{40}$' &&
tx_logs_topic2 =~ '^0x[0]{24}[a-fa-f0-9]{40}$' &&
tx_logs_topic3 == '' &&
tx_logs_data_int >= 1000000000000
```

### Expected Result

```
[
  {
    "blockHash": "0x7e18d1b403ba4620ac999b0616e10ed7b4731bd5f6137523e110513df6ec4863",
    "blockNumber": "0x11f5828",
    "contractAddress": "",
    "cumulativeGasUsed": "0x61fcfc",
    "effectiveGasPrice": "0x8481080f7",
    "from": "0xc08fb884576cc89957e9058ef11587c468c2952f",
    "gasUsed": "0x16db4",
    "logs": [
      {
        "address": "0xdac17f958d2ee523a2206206994597c13d831ec7",
        "blockHash": "0x7e18d1b403ba4620ac999b0616e10ed7b4731bd5f6137523e110513df6ec4863",
        "blockNumber": "0x11f5828",
        "data": "0x0000000000000000000000000000000000000000000000000000014476f26140",
        "logIndex": "0x83",
        "removed": false,
        "topics": [
          "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
          "0x000000000000000000000000367c42a6f261ec54ffbecf5f41c226be12a3dca0",
          "0x000000000000000000000000eae7380dd4cef6fbd1144f49e4d1e6964258a4f4"
        ],
        "transactionHash": "0x0f854f09fa38adca093432a69114bc988f8c50ac2143bc5987563c01bde8d24c",
        "transactionIndex": "0x75"
      }
    ],
    "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000008000000000000000000000000000000010000000000000000000000000000000400000000000000000000000008000000000000000000000000000000000000000000000000000000000000000000000000000000080000000000000010000000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000080000000000000000000000000000000000000000000000002000000000000000000000000000000000000000002000000000000000000000000000000000000000000020000000000000000000000000100000000",
    "status": "0x1",
    "to": "0x367c42a6f261ec54ffbecf5f41c226be12a3dca0",
    "transactionHash": "0x0f854f09fa38adca093432a69114bc988f8c50ac2143bc5987563c01bde8d24c",
    "transactionIndex": "0x75",
    "type": "0x2"
  }
]
```
