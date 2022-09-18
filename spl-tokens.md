# SPL tokens
Make sure you're using devnet or testnet for experiments!!!

### Create spl-token (hash representing token ID)
```
spl-token create-token
# Creating token 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp
```

### Create token account (holding tokens we will mint)
``` 
spl-token create-account 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp
# 5nZre57tEDpKnPLnS9sakyCXfXxuLZ6KZENRKqfsMN9o
```

### Mint tokens (create individual tokens)
```
spl-token mint 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp 100
```

### Check supply (tokens in existence)
```
spl-token supply 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp
```

### Check token account balance
```
spl-token balance 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp
```

### Burn token (destroy token)
```
spl-token burn 5nZre57tEDpKnPLnS9sakyCXfXxuLZ6KZENRKqfsMN9o 10
```

### Send spl-token
```
# action
spl-token transfer 
# token ID
3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp 
# amount
10 
# target receiver
DevS2De4VP1QZLm1W3FSWj1PuypodmT3493HBt63juv9
```

### Send spl-token (with creating/funding recepient account)
```
# action
spl-token transfer --fund-recipient 3Qekxw33Fe9NZ4txQMWmkAU2tiVrYHJAB61hQt4pkUnp 10  DevS2De4VP1QZLm1W3FSWj1PuypodmT3493HBt63juv9
```

### List all owned SPL-tokens
```
spl-token accounts
```