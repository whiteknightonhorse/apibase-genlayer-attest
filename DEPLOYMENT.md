# Live deployment

| | |
|---|---|
| Network | GenLayer Testnet Bradbury (chain id 4221) |
| Contract | [`0x7572cAB5B7Ba1547cDF259988582E3BBd8E2eaf8`](https://explorer-bradbury.genlayer.com/address/0x7572cAB5B7Ba1547cDF259988582E3BBd8E2eaf8) |
| Configured chain | Base (8453), USDC `0x833589fcd6edb6e08f4c7c32d4f71b54bda02913`, RPC `https://mainnet.base.org` |
| Receipts | `https://apibase.pro/r/<receipt_id>.json` |
| Frontend | https://apibase.pro/attest/?r=8bd61d9a8ebc8720770798237c469755 |
| Source | mirror of `integrations/genlayer-apibase-attest/` in [whiteknightonhorse/provek](https://github.com/whiteknightonhorse/provek/tree/ae9c152958edc33133a7d894475540b340885aaf/integrations/genlayer-apibase-attest) at commit `ae9c152` — the exact code that was deployed |

## Live attestations (2026-10-20)

| receipt | attest_id | GenLayer tx | result |
|---|---|---|---|
| [8bd61d9a…](https://apibase.pro/r/8bd61d9a8ebc8720770798237c469755.json) | `d1d1269f29e1e0b72bca8e96c9f12d5947b5b7e0adfb37d4baa17dc6fe91fb31` | `0x25588b775b8c2bc256b9bbce615e6c81d706fa895bae1de73857af271dc10367` | PASS · payment_matches |
| [c0eb6842…](https://apibase.pro/r/c0eb684260090f18513ceccc2c915e67.json) | `aab7abb09573cb4937136d985a9059844480f9b956dd61fc658887b448c9306e` | `0xeee3943bf9c2bd93f419672b210bf70c4c55220832c28622fa8692c33bcbf16d` | PASS · payment_matches |

Read them back without a wallet: `list_by_receipt(receipt_id)` and `get_attestation(attest_id)` on the contract, or open the frontend link above.
