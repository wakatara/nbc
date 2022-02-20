# Naive Blockchain

Simple p2p blockchain implementation in Rust with FloodSub (so, no real consensus algo. Simplified.).


Just a bit of educational programming for myself in Rust and with blockchain to understand the concepts.

3 Commands: 

1. ls p - prints p2p peers connected
2. ls c - prints the blockchain to point
3. create b <something> - mines a block on the node to set difficulty level

## Usage

Use `tmux` or separate terminals on your machine.

`RUST_LOG=info cargo run` in each pane or terminal

It'll print INFO messages to screen. You can use commands then as the terminal will also take input for the 3 commands above. 

use `create b HODL_to_the_Moon_FTW!` or similar start to kick off mining a block in each node. They'll mine blocks, flood to each other and add to their chain.


## TODOs

- [] TODO Implement better conensus algorithm for block completion and contention
- [] TODO Make the mining automated
- [] Ramp up difficulty level to represent controlled inflation as chain gets longer
- [] TODO Quiet the INFO print out matches to drop unhandled but know messages
- [] Reimplement in Golang to check ease and performance if each (GC etc.)
- [] In particular, implement without Rust's p2plib crate which does all heavy lifting here (Golang version?)
  





