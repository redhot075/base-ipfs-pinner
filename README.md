# Base IPFS Pinner Starter Kit\n\nPinata IPFS pinner for NFT metadata on Base L2. Upload JSON/image → pin → URI in contract.\n\n## Quick Start\n1. Install: `npm i pinata-sdk hardhat`\n2. Config: Edit pinata.config.js (API key/secret)\n3. Pin metadata: `node scripts/pin-metadata.js metadata.json`\n4. Deploy contract with IPFS URI: `npx hardhat run scripts/deploy.js --network baseSepolia`\n\nSee guide.

## Full Guide

### Pinata Setup
1. Sign up pinata.cloud → API key/secret
2. Pin metadata: 
3. Copy IPFS URI to contract _baseURI

### Deploy
1. 
2. 

### Example metadata.json
``
json
{
  "name": "Base Lobster #1",
  "image": "ipfs://QmImageHash",
  "attributes": []
}
```

**Pinata free tier: 1GB/100 pins.**
