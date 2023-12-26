## USDC Transfers on Polygon

### Description

Get a QuickAlert anytime there is a USDC transaction on Polygon Mainnet

### Blockchain & Network

Polygon Mainnet

### Expression Values

- `0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174` contract address of **USDC** on **Polygon Mainnet**

### Expression
```
tx_logs_address == '0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174'
```

### Expected Result

```
{
"block_number":51589765
"topic":"raw-polygon-mainnet"
"chain":"polygon-mainnet"
  "block":{
  "baseFeePerGas":"0x1b2d03f5fd"
  "difficulty":"0x18"
  "extraData":"0xd88301010083626f7289676f312e32302e3130856c696e757800000000000000ff2d69fd6af78b43ff65a6bcad5a34ce33777fa9f486683a9a66003d41c6218068bad679b9ddd003be7502a9367e6069ec966c5506b477095da9e11505bcfaa200"
  "gasLimit":"0x1c9c380"
  "gasUsed":"0xffc7b7"
  "hash":"0x43e94e8c1af8ffb6dca7c8124e3239f66ac7f14e3115c458c8ec4fc3a675f4a9"
  "logsBloom":"0x1c7c00f532850182fea8c004c4b4d040fa24530fee5d4b6809943c5a950b3d1d13281829ec45647641678810a11701710a02c330d31e6402a591f290612aa491884cb8e5182fc8e8e6e4abc9786aa0ab411505c4c571858cb5cbe2e697f7024268c4027986a750bcb89557d2a0068915808ebd55a100167da37be5ba49281469827322b680fd50200900d3ac171f99a0744b2fc1be15839a61434a76044229a0e24b0993d5709f044c22884e02dfbfa0f8f81c4b30b643132021b823405de7ddab3d52469261991d9b0788e2c84057604477ae422004c812c4578c9f2a71330b95d0a4a240408071240d2d8a6781778dc21080e752329859d44a501f46163d02"
  "miner":"0x0000000000000000000000000000000000000000"
  "mixHash":"0x0000000000000000000000000000000000000000000000000000000000000000"
  "nonce":"0x0000000000000000"
  "number":"0x3133285"
  "parentHash":"0xbd9d18c144beca2432bf1371b9e175d8b318ec344582bc9afc2693b562bd8e72"
  "receiptsRoot":"0x6bfd77cc6826c7017571efb6c19467903cbfc166cea9107fa35a66b8091d021b"
  "sha3Uncles":"0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347"
  "size":"0xd11f"
  "stateRoot":"0x7113091e77fb53f9b3c4a9411c61d579c92107a51b2156e406f9f18082bebbf3"
  "timestamp":"0x658b286d"
  "totalDifficulty":"0x36fd4ae4"
  "transactions": // Details of individual transactions in the block
  "transactionsRoot":"0xb280a097de28fba6851c4641e43a7b9e6eee61247443e38ed427a137a4ee8bcf"
  "uncles":[]
  }
  "receipts": [...]
}
```
