# Candy Machine User Interface Setup Guide

## Introduction
This guide offers a step-by-step walkthrough for configuring the user interface (UI) of your Candy Machine. The UI allows users to mint NFTs using the SPL token you've created, with transactions facilitated through their Phantom wallets.

## Prerequisites
Before you begin, ensure you have the following:

- A configured Candy Machine, with the necessary details in the `config.json` file, including price, quantity, symbol, seller fee basis points, SPL token account, SPL token, go-live date, and creator information.
- A Phantom wallet set up for minting.
- A newly created SPL token.

## Steps

### 1. SPL Token Setup
If you haven’t done so yet, create the SPL token according to the guidelines in Lesson Three and note its address.

### 2. Update Candy Machine Config
Edit your Candy Machine’s `config.json` file to update these fields:
- `splTokenAccount`: Enter the address of the created SPL token account.
- `splToken`: Enter the address of the SPL token.

### 3. UI Configuration
Follow the "Quick Node: Set Up a Minting Site" tutorial for guidance on creating a UI for your Candy Machine. This UI will allow users to connect their Phantom wallets and mint NFTs using the SPL token for payment.

### 4. Adjust Minting Logic
In your SPL project's minting logic (as detailed in Lesson Three), modify the code to ensure NFTs are minted to the Phantom wallet address. Alternatively, adjust the transfer function to send minted NFTs directly to the Phantom wallet.

### 5. Testing
Thoroughly test the entire setup by transferring or minting your SPL token to a Phantom account. Use the UI to mint NFTs, ensuring a smooth experience for users paying with the designated SPL token.
