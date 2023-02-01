# 💸 In-Browser Vending Machine

{% hint style="info" %}
#### Holding Requirements: 1 Wild Tangz = 500 NFT files at a time (unlimited refills)
{% endhint %}

This interface enables you to upload JSON-formatted metadata files (1 file per 1 asset), and configure a vending machine to monitor for UTXOs and process new mints. Profit vaults MUST be hardware (e.g., Ledger) for production use cases.&#x20;

**URL**: [https://www.wildtangz.com/vending-machine](https://www.wildtangz.com/vending-machine)&#x20;

**Status**: Production (Vasil) release&#x20;

**Documentation**: Tooltips overlay&#x20;

**Instructional Video**

{% embed url="https://youtu.be/lnSSzzT5T2c" %}

#### Sample JSON Metadata File

See below for a sample JSON file.  Note that the `721` and Policy ID wrappers are generated on the fly, so they should not be included in the uploaded file.

```
{
  "WildTangz 1": {
    "mediaType": "image/png",
    "project": "Wild Tangz",
    "fur": "Crimson",
    "body": "Default",
    "accessories": "None",
    "eyes": "Crying",
    "eyewear": "Monocle",
    "headwear": "Beret",
    "clothing": "Overalls",
    "mouth": "Cigarette",
    "name": "WildTangz 1",
    "background": "Carmine Pink",
    "image": "ipfs://QmdsAtotMCHAAPZEiw66H6kbDGpoEwy4pn4XTq6CbZQo5t"
  }
}
```

Each file should have exactly one asset in it.

**Codebase:** [https://github.com/thaddeusdiamond/cardano-nft-mint-frontend](https://github.com/thaddeusdiamond/cardano-nft-mint-frontend)
