---
slug: /sdk.multiwrapimpl
title: MultiwrapImpl class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## MultiwrapImpl class

> This API is provided as a preview for developers and may change based on feedback that we receive. Do not use this API in a production environment.

Multiwrap lets you wrap any number of ERC20, ERC721 and ERC1155 tokens you own into a single wrapped token bundle.

## Example

```javascript
import { ThirdwebSDK } from "@thirdweb-dev/sdk";

const sdk = new ThirdwebSDK("{{chainName}}");
const contract = sdk.getMultiwrap("{{contract_address}}");
```

## Constructors

| Constructor                                                                                                     | Modifiers | Description                                                                         |
| --------------------------------------------------------------------------------------------------------------- | --------- | ----------------------------------------------------------------------------------- |
| [(constructor)(network, address, storage, options, abi, contractWrapper)](./sdk.multiwrapimpl._constructor_.md) |           | **<i>(BETA)</i>** Constructs a new instance of the <code>MultiwrapImpl</code> class |

## Properties

| Property                                              | Modifiers           | Type                                                                                                                                                   | Description                           |
| ----------------------------------------------------- | ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------- |
| [abi](./sdk.multiwrapimpl.abi.md)                     |                     | typeof ABI                                                                                                                                             | **<i>(BETA)</i>**                     |
| [contractRoles](./sdk.multiwrapimpl.contractroles.md) | <code>static</code> | readonly \["transfer", "minter", "unwrap", "asset"\]                                                                                                   | **<i>(BETA)</i>**                     |
| [encoder](./sdk.multiwrapimpl.encoder.md)             |                     | [ContractEncoder](./sdk.contractencoder.md)&lt;MultiwrapContract&gt;                                                                                   | **<i>(BETA)</i>**                     |
| [estimator](./sdk.multiwrapimpl.estimator.md)         |                     | [GasCostEstimator](./sdk.gascostestimator.md)&lt;MultiwrapContract&gt;                                                                                 | **<i>(BETA)</i>**                     |
| [events](./sdk.multiwrapimpl.events.md)               |                     | [ContractEvents](./sdk.contractevents.md)&lt;MultiwrapContract&gt;                                                                                     | **<i>(BETA)</i>**                     |
| [metadata](./sdk.multiwrapimpl.metadata.md)           |                     | [ContractMetadata](./sdk.contractmetadata.md)&lt;MultiwrapContract, typeof MultiwrapContractSchema&gt;                                                 | **<i>(BETA)</i>**                     |
| [roles](./sdk.multiwrapimpl.roles.md)                 |                     | [ContractRoles](./sdk.contractroles.md)&lt;MultiwrapContract, typeof [MultiwrapImpl.contractRoles](./sdk.multiwrapimpl.contractroles.md)\[number\]&gt; | **<i>(BETA)</i>**                     |
| [royalties](./sdk.multiwrapimpl.royalties.md)         |                     | [ContractRoyalty](./sdk.contractroyalty.md)&lt;MultiwrapContract, typeof MultiwrapContractSchema&gt;                                                   | **<i>(BETA)</i>** Configure royalties |

## Methods

| Method                                                                                | Modifiers | Description                                                                                  |
| ------------------------------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------- |
| [getWrappedContents(wrappedTokenId)](./sdk.multiwrapimpl.getwrappedcontents.md)       |           | **<i>(BETA)</i>** Get the contents of a wrapped token bundle                                 |
| [unwrap(wrappedTokenId, recipientAddress)](./sdk.multiwrapimpl.unwrap.md)             |           | **<i>(BETA)</i>** Unwrap a wrapped token bundle, and retrieve its contents                   |
| [wrap(contents, wrappedTokenMetadata, recipientAddress)](./sdk.multiwrapimpl.wrap.md) |           | **<i>(BETA)</i>** Wrap any number of ERC20/ERC721/ERC1155 tokens into a single wrapped token |

**Signature:**

```typescript
export declare class MultiwrapImpl extends StandardErc721<MultiwrapContract>
```

**Extends:** [StandardErc721](./sdk.standarderc721.md)&lt;MultiwrapContract&gt;