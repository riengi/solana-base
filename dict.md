/# Solana dictionary

## Account
Data or executable program on Solana Ledger.

## Account owner
Address of the program that owns the account. Owner can modify the account.

## App
Front-end applicaiton

## Bank state
Result interpreting of all non-zero holding programs at given time. 

## Block
Set of entries covered by a vote. Leader can produce one block per slot.

## Blockhash
Unique hash that identifies the block. Computed from the last entry ID of the block. 

## Block height
Number of blocks beneath the current block. Genesis block height = 1

## Bootstrap validator
Validator that produces the genesis block.

## BFP loader
Solana program that owns and loads BFP smart contracts.

## Client
Any application that access Solana network cluster.

## Commitment
Expresses network confirmation of the blocks. 

## Cluster
Set of validators maintaining single ledger.

## Compute budget
Maximum number of compute units consumed by transaction. 

## Compute unit
Smallest unit of computational resources. 

## Confirmation time
Duration between ledger creating tick entry and confirmed block. 

## Confirmed block
Block that received a supermajority of ledger votes.

## Control plance
A gossip network connecting all nodes. 

## Cooldown period
Number of peochs afer stake has been deactivated affecting withdrawal time.

## Credit / Vote credit
A reward for validators. 

## Cross platform invocation (CPI)
Call from one smart program to another. 

## Data plane
Multicast network to efficiently validate entries and gain consensus.

## Drone
Off-chain service acting a s custody for a user private key. 

## Entry
Entry on the ledger, either a tick or a transaction entry.

## Entry ID
Resistant hash of the final contents of an entry.

## Epoch
Number of slots for which a leader schedule is valid.

## Fee Account
Accounts that pays for the transaction. Must be first account stated in the TXN.

## Finality
Happens when nodes representing 2/3 of the stake have a commmon root.

## Fork
Diverged ledger derived from common entries.

## Genesis block
The first blockch in the chain.

## Hash
Sequence of bytes representing digital 
fingerprint.

## Inflation
An increase of token supply caused by issuance of rewards for validation.

## Inner instruction
Calling one smart contract program from another. 

## Instruction
Smallest unit of execution logic in a program. It specifies: 1) which program to execute, 2) what accounts to read or modify, 3) additional data / input for the program. 1TXN = 1..n instructions. 1 instruction = 1..n CPI

## Keypair
Public key and corresponding private key for accessing the account. 

## Lamport
Native token, fragment of SOL, 1SOL = 10^9 LAMPORTS

## Leader
Validator that is allowed append entries to the ledger.

## Leader schedule
Sequence of validator public keys mapped to slots to determine which validator is the leader at any moment. 

## Ledger 
List of entries containing transactions signed by clients. Validator can have all blocks or just the latest. 

## Ledger vote
Hash of the validator's state at a given tick height. Proves that validator received and verified block and will not vote for conflicting block for certain time aka lockout period. 

## Light client
Client that can verify. It performs more dedger verification thin client and less than a validator. 

## Loader
Program with ability to inerpret binary encoding of other on-chain pograms. 

## Lockout
Duration of time for which validator is unable to vote for another fork. 

## Message
Structured contents of a transactions typically containing 1) header, 2) array of account messsages, 3) recent blockhash and 4) array of instructions. 

## Native token
Token used to track work done by nodes in a cluster. (SOL)

## Node
Computer participating in a cluster

## Node count
Number of validators in a cluster. 

## Proof of History (PoH)
Stack of proofs ensuring hat some data existed before the proof and given time passed before the previous proof. PoH can be verified in less time than it takes to produce. 

## Point
A weighted credit in a rewards regime. 

## Private key
Private key of a keypair. 

## Program
Executable code that interprets the instructions sent inside transactions. Similar to smart contracts on other chains. 

## Program derived account (PDA)
Account whose owner is a proram and thus is not controlled by a private key like other accounts. 

## Program ID
Public key of the account containing the program

## Prioritization fee
Additional user fee to prioritize transaction. 

## Public key
Public key of a keypair. 

## Rent
Fee paid by Accounts and Programs to store data on the blockchain. When accounts do not have enough balance to pay rent, they miy be Garbage Collected. 

## Rent exempt
Accounts that maintain more than 2 years with of rent payments in their account are considered "rent exempt" and will not incure the collection of rent. 

## Root
A block or slot that has reached maximum lockout on a validator. All ancestor blocks are also root transivively. Other blocks can be discarded. 

## Runtime
A component of a validator reponsible for program execution.

## Sealevel
Solana's parallel smart contracts runtime.

## Shred
A fraction of a block; the smallest unit sent between validators. 

## Signature
64-byte ed25519 signature of R (32-bytes) and S(32-bytes) with given parameters assuring no signature malleability. Each transaction must have at least on signature for fee account. First signature can be treated as transaction ID. 

## Skipped slot
A past slot that did not produce a block becaus of multiple reason (offline, ...). Any older not-rooted slot than latest rooted slot is basically skipped. 

## Smart contract
A program on a blockchain that can read and modify accounts over which it has control. 

## SOL
Native token of Solana cluster

## Solana Program Library (SPL)
Library of programs on Solana such as spl-token that facilitates token (and NFT) related operations. 

## Stake
Validator stake, can forfeit to the cluster if malicious validator bahavior can be proven. 

## Supermajority
2/3 of a cluster

## sysvar
System account. Provides cluster state information like current tick height, rewards points values, etc. Can be accessed via pubkey or by querying via a syscall. 

## Thin client
A type of client that trusts it is communicating witha valid cluster. 

## Tick
A ledger entry that estimates wallclock duration.

## Tick height 
The Nth tick in the ledger. 

## Token
Digitally transferable asset

## TPS
Transaction per second

## Transaction 
One or more instructions signed by a client, executed automatically with resulting in either success or a failure. 

## Transaction ID 
The first signature in a transaction. Unique identifier of the transaction across all ledger. 

## Transaction confirmations
Number of confirmed blocks since the transaction was accepted onto the ledger. Transaction is finalized when its block becomes a root. 

## Transactions entry
Set of transactions that may be executed in paralel. 

## Vaidator 
A full participant in a Solana network cluster that produces a new blocks. It also validates transactions. 

## Verifiable Delay Function (VDF)
Function that takes fixed amount of time to excecute producing proof that it ran which can be verified in less time than it took to produce. 

## Vote credit
Reward for validator in its vote account when validator reaches a root. 

## Wallet
Collection of keypairs that allows users to manage their funds.

## Warmup period
Number of periods after stake when stake is considered "activating". 




