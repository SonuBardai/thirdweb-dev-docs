---
slug: /reference/sdk.split
title: Split class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# Split class

Create custom royalty splits to distribute funds.

## Example

```javascript
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

const sdk = new ThirdwebSDK("{{chainName}}");
const contract = await sdk.getContract("{{contract_address}}", "split");
```

## Constructors

| Constructor                                                                                                      | Modifiers | Description                                               |
| ---------------------------------------------------------------------------------------------------------------- | --------- | --------------------------------------------------------- |
| [(constructor)(network, address, storage, options, abi, chainId, contractWrapper)](./sdk.split._constructor_.md) |           | Constructs a new instance of the <code>Split</code> class |

## Properties

| Property                                          | Modifiers             | Type                                                                                                                                                                                                                                                                                                                                                                                                                                                                     | Description                                                                     |
| ------------------------------------------------- | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------- |
| [abi](./sdk.split.abi.md)                         |                       | [Abi](./sdk.abi.md)                                                                                                                                                                                                                                                                                                                                                                                                                                                      |                                                                                 |
| [app](./sdk.split.app.md)                         |                       | [ContractAppURI](./sdk.contractappuri.md)&lt;SplitContract&gt;                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                 |
| [chainId](./sdk.split.chainid.md)                 | <code>readonly</code> | number                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |                                                                                 |
| [contractRoles](./sdk.split.contractroles.md)     | <code>static</code>   | readonly \["admin"\]                                                                                                                                                                                                                                                                                                                                                                                                                                                     |                                                                                 |
| [distribute](./sdk.split.distribute.md)           |                       | { (): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: () =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                                                                       | Distribute Funds                                                                |
| [distributeToken](./sdk.split.distributetoken.md) |                       | { (tokenAddress: string): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (tokenAddress: string) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                               | Distribute Funds                                                                |
| [encoder](./sdk.split.encoder.md)                 |                       | [ContractEncoder](./sdk.contractencoder.md)&lt;SplitContract&gt;                                                                                                                                                                                                                                                                                                                                                                                                         |                                                                                 |
| [estimator](./sdk.split.estimator.md)             |                       | [GasCostEstimator](./sdk.gascostestimator.md)&lt;SplitContract&gt;                                                                                                                                                                                                                                                                                                                                                                                                       |                                                                                 |
| [events](./sdk.split.events.md)                   |                       | [ContractEvents](./sdk.contractevents.md)&lt;SplitContract&gt;                                                                                                                                                                                                                                                                                                                                                                                                           |                                                                                 |
| [metadata](./sdk.split.metadata.md)               |                       | [ContractMetadata](./sdk.contractmetadata.md)&lt;SplitContract, typeof SplitsContractSchema&gt;                                                                                                                                                                                                                                                                                                                                                                          |                                                                                 |
| [roles](./sdk.split.roles.md)                     |                       | [ContractRoles](./sdk.contractroles.md)&lt;SplitContract, (typeof [Split.contractRoles](./sdk.split.contractroles.md))\[number\]&gt;                                                                                                                                                                                                                                                                                                                                     |                                                                                 |
| [withdraw](./sdk.split.withdraw.md)               |                       | { (walletAddress: string): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (walletAddress: string) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; }                                             | Withdraw Funds                                                                  |
| [withdrawToken](./sdk.split.withdrawtoken.md)     |                       | { (walletAddress: string, tokenAddress: string): Promise&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;; prepare: (walletAddress: string, tokenAddress: string) =&gt; Promise&lt;[Transaction](./sdk.transaction.md)&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;&gt;&gt;; } | Triggers a transfer to account of the amount of a given currency they are owed. |

## Methods

| Method                                                                                  | Modifiers | Description                                                             |
| --------------------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------------- |
| [balanceOf(address)](./sdk.split.balanceof.md)                                          |           | Get Funds owed to a particular wallet                                   |
| [balanceOfAllRecipients()](./sdk.split.balanceofallrecipients.md)                       |           | Returns all the recipients and their balances in the native currency.   |
| [balanceOfToken(walletAddress, tokenAddress)](./sdk.split.balanceoftoken.md)            |           | Get non-native Token Funds owed to a particular wallet                  |
| [balanceOfTokenAllRecipients(tokenAddress)](./sdk.split.balanceoftokenallrecipients.md) |           | Returns all the recipients and their balances in a non-native currency. |
| [getAddress()](./sdk.split.getaddress.md)                                               |           |                                                                         |
| [getAllRecipients()](./sdk.split.getallrecipients.md)                                   |           | Get Recipients of this splits contract                                  |
| [getRecipientSplitPercentage(address)](./sdk.split.getrecipientsplitpercentage.md)      |           | Get the % of funds owed to a given address                              |
| [onNetworkUpdated(network)](./sdk.split.onnetworkupdated.md)                            |           |                                                                         |

**Signature:**

```typescript
export declare class Split implements UpdateableNetwork
```

**Implements:** UpdateableNetwork