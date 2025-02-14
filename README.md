# Detyre-Kursi
# README.md

# Simple Blockchain Implementation

## Overview
This project is a basic blockchain implementation in Python. It includes:
- A `Block` class that defines the structure of a block.
- A `Blockchain` class that manages the chain and implements Proof of Work.
- A function to validate the blockchain’s integrity.

## Requirements
- Python 3.x

## Installation
```sh
# Clone the repository
git clone <repo-url>
cd blockchain-project

# Run the script
python blockchain.py
```

## Features
- Adds new blocks to the chain.
- Implements Proof of Work with adjustable difficulty.
- Ensures blockchain integrity.

## Example Usage
```python
blockchain = Blockchain()
block1 = Block(1, blockchain.get_latest_block().hash, time.time(), "Transaction Data")
blockchain.proof_of_work(block1)
blockchain.add_block(block1)
print("Blockchain is valid:", blockchain.validate_chain())
```

# Git Automation Script
```sh
#!/bin/bash
# git_auto.sh: Automate Git commits & pushes

git add .
git commit -m "Updated blockchain project"
git push origin main
```

## Usage
```sh
chmod +x git_auto.sh
./git_auto.sh
