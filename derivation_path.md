# Derivation path on Solana

### Basics

* Solana implicitly includes 44'/501' and follows BIP44 specification
* any derived keys are Solana keys (Coin type 501)
* format  m/purpose/coin_type/account/change/address_index
* there are infinitely many derivation paths
* Sollet and Phantom uses derivation path m/44'/501'/0'/0
* Solflare uses derivation path m/44'/501'/0
* change address is used for BTC, not for Solana
