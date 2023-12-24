## EAS Attestation Event

### Description

Get a QuickAlert when a specific EAS schema attestation is emitted

This QuickAlert listens to the `Attested` event from EAS and can be filtered to a specific schema.

Here's the event definition, `Attested (index_topic_1 address recipient, index_topic_2 address attester, bytes32 uid, index_topic_3 bytes32 schema)`.

### Blockchain & Network

Ethereum Mainnet.
Optimism Mainnet.

> **Note:** To support other EVM-compatible network, change the `tx_logs_address` to the **contract address** of EAS on that specific network.
>
> Also make sure to change the `tx_logs_data_int` to reflect the **number of decimals** in the USDT and USDC contract.

### Expression Values

- `0x4200000000000000000000000000000000000021` contract address of **EAS** on **Optimism Mainnet**
- `0xA1207F3BBa224E2c9c3c6D5aF63D0eb1582Ce587` contract address of **EAS** on **Ethereum Mainnet**
- `0x8bf46bf4cfd674fa735a3d63ec1c9ad4153f033c290341f3a588b75685141b35` Topic hash of **Attested** event

### Expression

```
tx_logs_address == '0x4200000000000000000000000000000000000021' &&
tx_logs_topic0 == '0x8bf46bf4cfd674fa735a3d63ec1c9ad4153f033c290341f3a588b75685141b35'
```
Optionally you can filter by a specific schema
```
...  &&
tx_logs_topic3 == SPECIFIC_SCHEMA_UID
```

### Expected Result

```
[
  {
    "blockHash":"0x759b4387e39645285ccc15e39ada134fd13827e5aebd0e6928f8630c28906af4"
    "blockNumber":"0x6c9e503"
    "contractAddress":NULL
    "cumulativeGasUsed":"0x1de798"
    "effectiveGasPrice":"0x4264a9"
    "from":"0xa5ba45f484bc67fe293cf01f7d92d5ba3514dd42"
    "gasUsed":"0x7628e"
    "l1Fee":"0x65426a26229f"
    "l1FeeScalar":"0.684"
    "l1GasPrice":"0x46d67f742"
    "l1GasUsed":"0x2170"
    "logs":[
      {
        "address":"0x4200000000000000000000000000000000000021"
        "topics":[
          "0x8bf46bf4cfd674fa735a3d63ec1c9ad4153f033c290341f3a588b75685141b35",
          "0x000000000000000000000000a5ba45f484bc67fe293cf01f7d92d5ba3514dd42",
          "0x00000000000000000000000038e9ef91f1a96aca71e2c5f7abfea45536b995a2",
          "0x94cb5f1d1fae19f01f86fecf432aff882f588c0671186e3f90feeea4fa999d38",
        ]
        "data":"0x2b513338cdaa87af778235493fa24024b668c6cfcdf8319c425ecf5df9e315d3"
        "blockNumber":"0x6c9e503"
        "transactionHash":"0x437144950c3e31bc70e3deea02d2c87dc8ece5c3e076764fdafd2136ab701151"
        "transactionIndex":"0xc"
        "blockHash":"0x759b4387e39645285ccc15e39ada134fd13827e5aebd0e6928f8630c28906af4"
        "logIndex":"0x21"
        "removed":false
      }
    ]
    "logsBloom":"0x00000000000000000000200040000000000000000000000000000000000000000000000000000000000008100000000000010000000000000040000000000000000000000000000000000000000000000000000000000008000000000000000000000010000000000000040000000000000000000000002000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008010000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000000800000004000000000000200040000000000000000004000000000000"
    "status":"0x1"
    "to":"0x38e9ef91f1a96aca71e2c5f7abfea45536b995a2"
    "transactionHash":"0x437144950c3e31bc70e3deea02d2c87dc8ece5c3e076764fdafd2136ab701151"
    "transactionIndex":"0xc"
    "type":"0x2"
  }
]
```
