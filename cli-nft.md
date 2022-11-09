#  NFT / SPL tokens
Make sure you're using devnet or testnet for experiments !!!
NFTs on Solana are basically SPL tokens with supply = 1 and 0 decimals

### Create NFT token
```
spl-token create-token --decimals 0
```

### Create NFT token account (account holding the token)
``` 
spl-token create-account ByjyBvvvJRvu2YT9iEpccFCBSMmDwKpAaAJh3rL9EM6Q
```

### Mint NFT token
```
spl-token mint ByjyBvvvJRvu2YT9iEpccFCBSMmDwKpAaAJh3rL9EM6Q 1
```

### Disable more minting 
```
spl-token authorize ByjyBvvvJRvu2YT9iEpccFCBSMmDwKpAaAJh3rL9EM6Q mint --disable
```

### Check token account balance
```
spl-token balance ByjyBvvvJRvu2YT9iEpccFCBSMmDwKpAaAJh3rL9EM6Q
```

### Send NFT (with creating/funding recepient account)
```
spl-token transfer --fund-recipient ByjyBvvvJRvu2YT9iEpccFCBSMmDwKpAaAJh3rL9EM6Q 1  DevS2De4VP1QZLm1W3FSWj1PuypodmT3493HBt63juv9
```

### List all NFTs
```
spl-token accounts
```