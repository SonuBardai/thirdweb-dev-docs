---
slug: /reference/sdk.staticjsonrpcbatchprovider
title: StaticJsonRpcBatchProvider class
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# StaticJsonRpcBatchProvider class

**Signature:**

```typescript
export declare class StaticJsonRpcBatchProvider extends providers.StaticJsonRpcProvider
```

**Extends:** providers.StaticJsonRpcProvider

## Constructors

| Constructor                                                                                    | Modifiers | Description                                                                    |
| ---------------------------------------------------------------------------------------------- | --------- | ------------------------------------------------------------------------------ |
| [(constructor)(url, network, batchOptions)](./sdk.staticjsonrpcbatchprovider._constructor_.md) |           | Constructs a new instance of the <code>StaticJsonRpcBatchProvider</code> class |

## Properties

| Property                                                                                | Modifiers | Type                                                                                                                                                                                   | Description |
| --------------------------------------------------------------------------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------- |
| [\_pendingBatch](./sdk.staticjsonrpcbatchprovider._pendingbatch.md)                     |           | Array&lt;{ request: { method: string; params: Array&lt;any&gt;; id: number; jsonrpc: "2.0"; }; resolve: (result: any) =&gt; void; reject: (error: Error) =&gt; void; }&gt; &#124; null |             |
| [\_pendingBatchAggregator](./sdk.staticjsonrpcbatchprovider._pendingbatchaggregator.md) |           | NodeJS.Timer &#124; null                                                                                                                                                               |             |

## Methods

| Method                                                           | Modifiers | Description |
| ---------------------------------------------------------------- | --------- | ----------- |
| [send(method, params)](./sdk.staticjsonrpcbatchprovider.send.md) |           |             |