# NFT Marketplace Contract

This contract allows users to list their NFTs for sale and other users to buy them. It utilizes the ERC721 standard for NFTs and includes basic marketplace functionalities.

## Features

- List NFTs for sale by transferring them to the marketplace contract.
- Users can buy listed NFTs by paying the specified price.
- The contract tracks unsold and sold items separately.

## How to Use

1. Deploy the contract and ensure it has access to the required ERC721 contract.
2. Use the `listNFT()` function to list an NFT for sale.
3. Other users can purchase listed NFTs using the `buyNFT()` function by sending the correct price.
4. Use `fetchMarketItems()` to retrieve the current unsold items.

## Security Considerations

- Ensure the marketplace is trusted before transferring NFTs.
- The contract uses a non-reentrant guard to prevent reentrancy attacks during the purchase process.
