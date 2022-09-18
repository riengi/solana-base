# Keygen 

### Generate Account keys
```
solana-keygen new -o ./key.json
```

### Account balance
```
solana balance -k key.json
```

### Account airdrop (on devnet)
```
solana airdop 1 -k key.json
```

### Changing default keypair
```
solana config set --keypair key.json
```
Now you don't need "-k key.json" for most commands

### Send SOL to another account
```
solana transfer DevS2De4VP1QZLm1W3FSWj1PuypodmT3493HBt63juv9
```

### Send SOL to another unfunded account
```
solana transfer DevS2De4VP1QZLm1W3FSWj1PuypodmT3493HBt63juv9 --allow-unfunded-recipient
```