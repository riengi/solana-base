# CLI Solana Staking

## Create stake account
```
solana create-stake-acount -from <KP> stake.json <AMOUNT> --stake-authority <KP> --withdraw-authority <KP>
```

## Stake acount status
```
solana stake-account <ADDRES>
```

## List validators
```
solana validators
```

## Delegate / Activate stake
solana delegate-stake --stake-authority <KP> <KP_STAKE_ACCOUNT> <VALIDATOR>


## Unstake / deactivate stake
```
solana deactivate-stake 
--stake-authority <KP> <STAKE_ACCOUNT_ADDRESS>
```
## Withdraw stake
```
solana withdraw-stake --withdraw-authority <KP> <STAKE_ACCOUNT> <RECEPIENT_ADDRESS> <AMOUNT>
```
