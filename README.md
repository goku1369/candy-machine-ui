# Guide for Setting Up the Candy Machine User Interface

## Overview
This guide offers a detailed walkthrough for configuring the user interface (UI) of your Candy Machine. The UI facilitates the minting of NFTs using the SPL token you've generated, with users leveraging their Phantom wallets for the minting process.

## Prerequisites
Before proceeding, ensure you have the following prerequisites in place:

- A properly configured Candy Machine with specific details in its `config.json` file. This includes information such as price, quantity, symbol, seller fee basis points, SPL token account, SPL token, go-live date, and creator details.
- A designated Phantom wallet for the minting process.
- A newly created SPL token.

## Steps

### 1. SPL Token Setup
If not done already, create the SPL token following the guidelines outlined in Lesson Three. Take note of the SPL token's address.

### 2. Update Candy Machine Config
Edit your Candy Machine's `config.json` file and update the following fields:
- `splTokenAccount`: Replace it with the address of the created SPL token account.
- `splToken`: Replace it with the SPL token address.

### 3. UI Configuration
Refer to the "Quick Node: Set Up a Minting Site" tutorial for instructions on creating a UI for your Candy Machine. This UI empowers users to connect their Phantom wallets and mint NFTs using the SPL token as payment.

### 4. Adjust Minting Logic
Within your SPL project's minting logic (as per Lesson Three), make the necessary modifications to mint NFTs to the Phantom wallet address or adapt the transfer function to deliver minted NFTs to your Phantom wallet.
