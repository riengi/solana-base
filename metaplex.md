# Metaplex
https://docs.metaplex.com/
https://github.com/metaplex-foundation/js#readme


## Parts
* Wallet acount (owned by System Program)
* Token account (owned by Token Proram)
* Mint account (owned by Token Program)
* (PDA) Metadata Acount (owned by Token Metadata Program)
* Off-chain (Arweave) JSON Object (referenced by  URI from Metadata Program )
* (PDA) Master Edition Account 


## Mint Accout
* Owner: Token Program
* Mint authority : MEA
* Supply : 1
* Decimals: 0
* Freeze Authority: MEA

## Metadata account
* Key
* Update Authority
* Mint
* Name
* Symbol
* URI
* Seller Fee Basis Points
* Creators
* Primary Sale Happened
* IsMutable
* Edition Nonce
* Token Standard
* Collection
* USES
* Collection Details

## NFT tokens
* supply = 1 (Mint account)
* amount = 1 (Token Account)
* decimals = 0 (Mint Account)
* no mint authority (Mint Account)

## Master Edition Account (MEA)
* owner: Token Metadata Program
* Key : MasterEditionV2
* Supply
* Max Supply
