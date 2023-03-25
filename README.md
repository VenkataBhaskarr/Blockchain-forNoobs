# Blockchain-forNoobs

This repository would contains everything i will learn about the blockchain technology escpecially the solana blockchain.


# Solana Blockchain
Now let's beign the show i will just skimm through the knowledge... for more reference watch this video

## Introduction

Apart from other operations we would discuss about creating a customized token using special token program/smart contract that is developed by the solana team and deployed on the solana block chain itself.

1. In order to create  a token you should first generate your keypair/bank wallet through solana CLI

``` solana-keygen new ```
this would create a new keypair and stores in a particular file in your system

2. Next you need to create a mint using the smart contract we discussd above in order to do that we should pay some gas fee....and here comes the most important part
3. there are many environments in solana blockchain like the main production envirtonmetn mainnet , devnet , testnet and etc.. we need to change to devnet where the solana doesnt have any mobnetarty value and we can airdrop sol to our acccount
4. resuming the secind step after airdroping some sol to yourr bank wallet create the mint using smart contract

``` spl-token create-token ```

5. now create a associated token account for your bank account 

``` spl-token create-account <MINT_ADDRESS>

6. No you have to mint the number of tokens ytou want 

``` spl-token mint <MINT_ADDRESS> 10000

7. Now you have to transfer some of these tokens to you bak associated token 

``` spl-token transfer <MINT_ADDRESS> <AMOUNT> <PUBLIC_ADDRESS_OF_RECIPIENT>

8. This will automatically generates the associated token account for users for this particular token to store

9.generally every wallet is like a gpay and associated token account is like a bank account where the constraint is the associated toke. account can only store one specific token and the the end user should also follow the same criteria

10. Naming and adding the meta data to our tokens will be discussed shortly




## Assignment 1
Objective -  creating a airdrop website

1. user enters the recipeint public address and the amount he wants and click on submit 
2. usually how this would happen in cli is 
spl-token transfer <MINT_ADDRESS> <AMOUNT> <RECIPEINT_ADDRESS>

3. 


## Assignment 2

