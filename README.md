# **Airdrop Recovery Guide for Compromised Ethereum Wallets**

This guide explains how to safely claim airdropped tokens from wallets where you've lost access to the private keys but still control the address. The method uses specialized tools to intercept pending transactions and securely transfer assets before attackers can steal them.

## **What You'll Need**
- The compromised Ethereum wallet address
- A newly created secure wallet (with fresh seed phrase)
- A considerable amount of ETH in your new wallet for gas fees
- Chrome or Brave browser for extension 
- Basic understanding of MetaMask and Ethereum transactions

## **Required Tools**
| Tool         |           Purpose                                   | Link |
|--------------|-----------------------------------------------------|----------------
| Interceptor  | Monitors pending transactions                       | [dark.florist](https://dark.florist) |
| Lunara       | Handles secure token transfers                      | (Built into Interceptor) |
| Bouquet      | Bundles transactions securely                       | [bouquet.dark.florist](https://bouquet.dark.florist) |

## **Step-by-Step Instructions**

1. **Setup Transaction Monitoring**
   - Open [Interceptor](https://dark.florist)
   - Connect MetaMask in read-only mode
   - Enter your compromised wallet address
   - Remove any default test accounts
   - Activate scanning with the "Make Me Rich" button

2. **Prepare the Transfer**
   - When an airdrop claim is detected, switch to Lunara
   - Configure:
     - Source: Your compromised wallet
     - Destination: Your new secure wallet  
     - Token: Contract address (verify on Etherscan)
   - Set appropriate gas limits 

3. **Execute the Recovery**
   - Open [Bouquet](https://bouquet.dark.florist) separately
   - Connect your secure wallet (not the compromised one)
   - Import the transaction data from Interceptor
   - Set priority fee to 2x current network rate
   - Review all details carefully before sending

4. **Post-Recovery Security**
   - Immediately verify the transfer on Etherscan
   - Revoke all token approvals at [revoke.cash](https://revoke.cash)
   - For large amounts, consider transferring to another fresh wallet

## **Important Notes**
- **Timing Matters:** Execute when network congestion is low (check [gas tracker](https://etherscan.io/gastracker))
- **Security First:** Never reuse the compromised wallet for anything
- **Test First:** Try with small amounts when possible

## **Troubleshooting Common Issues**
- If transactions fail, increase gas limit by 20% and retry
- For missing tokens, double-check the contract address
- Against front-running, use higher priority fees or Flashbots

AND YOU SHOULD HAVE YOUR CLAIMED AIRDROP IN YOUR NEW WALLET 
