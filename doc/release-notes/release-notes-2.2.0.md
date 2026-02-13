Notable changes
===============

Network Upgrade 4: Canopy
--------------------------

The code preparations for the Canopy network upgrade are finished and included in this release. The following ZIPs are being deployed:

- [ZIP 207: Funding Streams](https://zips.z.cash/zip-0207)
- [ZIP 211: Disabling Addition of New Value to the Sprout Value Pool](https://zips.z.cash/zip-0211)
- [ZIP 214: Consensus rules for a Zcash Development Fund](https://zips.z.cash/zip-0214)

Canopy will activate on testnet at height TODO, and can also be activated at a specific height in regtest mode by setting the config option `-nuparams=0xe9ff75a6:HEIGHT`.

**Important update:**  
The originally planned Canopy mainnet activation height (**1680000**) has been **postponed**.

Canopy will activate on **mainnet at block height 1735000**. Activation is **immediate at this height**, with no gradual enforcement or signaling period.

**Mining pools and services must upgrade before block 1735000.**  
Nodes or pool software that do not support Canopy consensus rules (including Funding Streams in the coinbase transaction) will begin producing or accepting invalid blocks at activation.

See [ZIP 251](https://zips.z.cash/zip-0251) for additional information about the deployment process for Canopy.
