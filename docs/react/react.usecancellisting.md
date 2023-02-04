---
slug: /react.usecancellisting
title: useCancelListing() function
hide_title: true
displayed_sidebar: react
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

## useCancelListing() function

> This feature is currently in beta and may change based on feedback that we receive.

Use this to cancel a listing on your marketplace contract.

## Example

```jsx
const Component = () => {
  const {
    mutate: cancelListing,
    isLoading,
    error,
  } = useCancelListing(">>YourMarketplaceContractInstance<<");

  if (error) {
    console.error("failed to cancel auction listing", error);
  }

  return (
    <button disabled={isLoading} onClick={() => cancelListing()}>
      Cancel Auction Listing!
    </button>
  );
};
```

**Signature:**

```typescript
export declare function useCancelListing(
  contract: RequiredParam<Marketplace>,
): import("@tanstack/react-query").UseMutationResult<
  Omit<
    {
      receipt: import("@ethersproject/abstract-provider").TransactionReceipt;
      data: () => Promise<unknown>;
    },
    "data"
  >,
  unknown,
  Pick<AuctionListing | DirectListing, "id" | "type">,
  unknown
>;
```

## Parameters

| Parameter | Type                                                         | Description                           |
| --------- | ------------------------------------------------------------ | ------------------------------------- |
| contract  | [RequiredParam](./react.requiredparam.md)&lt;Marketplace&gt; | an instance of a Marketplace contract |

**Returns:**

import("@tanstack/react-query").UseMutationResult&lt;Omit&lt;{ receipt: import("@ethersproject/abstract-provider").TransactionReceipt; data: () =&gt; Promise&lt;unknown&gt;; }, "data"&gt;, unknown, Pick&lt;AuctionListing \| DirectListing, "id" \| "type"&gt;, unknown&gt;

a mutation object that can be used to cancel a listing