![alt text](https://github.com/bitDubai/media-kit/blob/master/MediaKit/Fermat%20Branding/Fermat%20Logotype/Fermat_Logo_3D.png "Fermat Logo")

# Fermat Token Platform

## Introduction

The scope and functionality related [Fermat Tokens](https://github.com/Fermat-ORG/fermat/blob/master/FERMAT-WHITE-PAPER.md) in Fermat.org is still under review and is wider than what this bounty will focus on.

There is a business need to start issuing Fermat Tokens manually, and the creation of this platform is to fullfill this need. Fermat Token Platform is expected to evolve greatly over time.

## Scope

### Fermat Token Platform

A new platform will be created that will include:

* new Fermat Token Wallet

* new Actor and Identity **Fermat Token Issuer**, that will extend **Asset Issuer** identity and actor.

* New Transactions that will be used to define basic information for the Fermat Tokens and a heavily usage of DAP Transactions.


### New Digital Asset type: Fermat Token

We will be adding a new type of *Digital Asset* called **Fermat Token** that will have an specific *Digital Asset Contract*.

Current *Digital Asset Contract* properties include:

* Expiration Date: which can be null.
* Allow Redemption: indicates if it can be redeemable in a Redemption Point. Token Assets will **not be** reedemable.
* Allow Transfer: indicates if it can be transfered between users. Token Assets will be transferable.
* Allow Selling: indicates if it can be selled and buyed between users. Token assets will be allowed for selling.

Specific Fermat Token Assets contract properties will include:

* Fermat Token amount: indicating the amoun of Fermats Tokens this asset represents.

### Transactions

Current transactions supported at DAP are:

* Asset Issuing

* Asset Distribution

* Asset Redemption: this transaction type will not be supported for Fermat tokens.

* Asset Transfer

* Asset Sell


Changes should be included in all transactions types to validate identity of Asset Issuer. *See Current Issues* section.

### Fermat Token Wallet

A new type of Wallet will be added to store the issued Fermat Tokens and support the DAP Transactions execution.

### Fermat Token Factory

that will allow the manual creation of **Fermat Tokens** defining the contract properties and DAP Transactions.


### Current issues

#### Asset Issuer Identity Registration

Currently, the platforms allows the creation of **Asset Issuer** identities without any type of control. Meaning that anyone can register an **Asset Issuer** identity choosing whatever name. Identity creation happens locally on each device and assets are created using that identity.

**Assets Users** later receive those assets without validating the authenticity of the **Asset Issuer** that sent the asset.

Since *Fermat.org* will be the **Asset Issuer** identity creating the **Fermat Tokens** we need to provide validation to the platform to allow the issuing of Fermat to this unique identity and provide mechanisms for **Asset Users** to accept them.

These validations shoulds exists not only for the new Fermat Tokens platform but for every **Asset Issuer** identity creation in DAP platform.

##### Blockchain registration proposal:

* The creation of the Asset Issuer identity is registered in the Bitcoin Blockchain with an **Asset Issuer Registration** transaction that includes in the OP_Return field the public key of the identity.

* The Asset factory, before allowing the creation of an asset, request the **Asset Issuer Registration** transaction to validate it existence and compares the Asset Issuer hash and request the identity private key to sign  the issued asset.

* This ensures that every asset created is owned by the registered **Asset Issuer** identity.

* When an Asset User or Redeem Point receives an asset, an additional validation to verify that the asset is from a registered **Asset Issuer** should be added by getting the **Asset Issuer Registration** transaction from the blockchain. Since the platform already validates that the Asset is the same that was issued by the Asset Issuer during the Issuing process, no additional validations are necessary to certify the asset is from the registered issuer.

* We should provide methods to export and import the **Asset Issuer** registered identity to be able to use it on any device.

##### P2P validation of the Identity

* Registered identities should be propagated accross the P2P network of Fermat devices and stored locally to provide control on **Asset Issuer** name, picture and data so that only one identity with that information exists.

* Before registering an **Asset Issuer** on Blockchain, the platform must validate no other issuer already exits with the same parameters.

* Another option could be to store each registered Identity on a centralized server to validate that only one identity with the defined information exists.

By adding these controls, a single, unique and validated **Asset Issuer** identity representing  a issuing role, would exists in the P2P network.

## Timeline

[To be define after final review of this document]

## Evaluation
[To be define after final review of this document]

## Distribution
[To be define after final review of this document]