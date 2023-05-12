---
slug: /reference/sdk.getcontractparams
title: GetContractParams type
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# GetContractParams type

**Signature:**

```typescript
export type GetContractParams<TContractType extends PrebuiltContractType> = {
  address: AddressOrEns;
  contractTypeOrAbi?: PrebuiltContractType | ContractInterface | TContractType;
  network: NetworkInput;
  storage?: ThirdwebStorage;
  sdkOptions?: SDKOptions;
};
```

**References:** [PrebuiltContractType](./sdk.prebuiltcontracttype.md), [AddressOrEns](./sdk.addressorens.md), [NetworkInput](./sdk.networkinput.md), [SDKOptions](./sdk.sdkoptions.md)