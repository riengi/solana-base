# Solana Programming Model


## Accounts
Account : basic building block for state on Solana

Address (Public Key) : maps locations of accounts

Account owner: Account that modify its data

Data on Solana: byte representation of anything less than 10MB

Program (Smart Contract): Account marked as executable 

---
## Transaction
Transaction : can execute executable code within Program 

Transaction content: 
* list signatures
* message
    * header
    * addresses
    * recent_blockhash
    * list of instructions


---
## Instructions
Instruction content:
* program_id
* accounts
* instruction_data

Program_id is address of program that the instruction is for

Accounts is a list of accounts that needs to be loaded by runtime

Instruction data are specific data for the instruction. 

Example: 

Transfer SOL instruction
* program_id : 1111111111111111111 (System Program)
* accounts: [Alice, Bob, System Program]
* instruction_data

Debit address needs to be signed
Credit address doesn't need to be signed (exception)

---

## Program Derived Addresses (PDA)
Addresses that can be derived from seeds. PDA accounts don't have private keys. 

If program needs to sign transactions for PDA, it uses seed to sign it. 

Program (Smart contract) owns account data for our DAAP so it can modify it. 


## Complete flow (general)
* Client signs transaction with private key of an account it desires to change
* Program checks if it's owner of the account AND if private key of the account is authorized the change 
* Program modifies data (if ^ is true)

## System program
* 1111111111111111
* default owner, responsible for creating accounts

## Creating new account flow 
* user with public key generates new keypair
* user regiesteres public key with system program
* user authorized debit from the original account to pay for the new account's rent
* user signs the instruction with both private keys
* system program will create that account for you
* system program marks itself as a program owner
* system program will sign the account with public key 