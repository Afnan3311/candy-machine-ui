# Candy Machine User Interface Setup Guide 

## Introduction
This guide provides a comprehensive walkthrough for configuring the user interface (UI) of your Candy Machine. The UI facilitates NFT minting using the SPL token you've generated, with users utilizing their Phantom wallets for the minting process.

## Prerequisites
Ensure you have the following prerequisites before proceeding:

- A configured Candy Machine with specific details in its `config.json` file, including price, quantity, symbol, seller fee basis points, SPL token account, SPL token, go-live date, and creator details.
- A Phantom wallet designated for minting.
- A newly created spl token

## Steps

### 1. SPL Token Setup
If not done already, create the SPL token in accordance with Lesson Three guidelines, and take note of the SPL token's address.

### 2. Update Candy Machine Config
Edit your Candy Machine's `config.json` file, updating the following fields:
- `splTokenAccount`: Replace with the address of the created SPL token account.
- `splToken`: Replace with the SPL token address.

### 3. UI Configuration
Refer to the "Quick Node: Set Up a Minting Site" tutorial for instructions on creating a UI for your Candy Machine. This UI empowers users to connect their Phantom wallets and mint NFTs using the SPL token as payment.

### 4. Adjust Minting Logic
Within your SPL project's minting logic (as per Lesson Three), make the necessary modifications to mint NFTs to the Phantom wallet address or adapt the transfer function to deliver minted NFTs to your Phantom wallet.

### 5. Testing
Thoroughly test the entire setup by transferring or minting your SPL token to a Phantom account. Utilize the UI to mint NFTs, ensuring a seamless process for users paying in the designated SPL token.

