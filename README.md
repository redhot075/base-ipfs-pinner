# Base IPFS Pinner Starter Kit

Pinata IPFS pinner for NFT metadata on Base L2. Upload JSON/image → pin → URI in contract.

## Quick Start

1. **Install:**
   ```
   npm init -y
   npm i pinata-sdk hardhat @nomicfoundation/hardhat-toolbox
   ```

2. **Config:** Edit `scripts/pin-metadata.js` (Pinata API key/secret).

3. **Pin metadata:**
   ```
   node scripts/pin-metadata.js metadata.json
   ```

4. **Deploy contract with IPFS URI:**
   ```
   npx hardhat run scripts/deploy.js --network baseSepolia
   ```

## Full Guide

### Pinata Setup
1. Sign up [pinata.cloud](https://pinata.cloud) → API key/secret.
2. Pin metadata → copy `ipfs://Qm...` to contract `_baseURI`.

### Deploy
1. Compile: `npx hardhat compile`
2. Deploy: `npx hardhat run scripts/deploy.js --network baseSepolia`
3. Verify: Base Sepolia explorer (tx hash).

### Example metadata.json
```json
{
  "name": "Base Lobster #1",
  "description": "On-chain lobster NFT",
  "image": "ipfs://QmImageHash",
  "attributes": [{"trait_type": "Stage", "value": "Egg"}]
}
```

**Pinata free tier: 1GB/100 pins.** Base ready! 🚀
