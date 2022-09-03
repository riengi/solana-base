# Solana Native

## Entrypoint
Entry point function for the Solana Program
```rust
// lib.rs
entrypoin!(process_instruction)
```

## Process instruction function
Function that takes transaction instruction and process it.

```rust
fn process_instruction(
    program_id: &Pubkey,
    account: &[AccountInfo],
    instruction_data: &[u8]
) -> ProgramResult {

}
```


