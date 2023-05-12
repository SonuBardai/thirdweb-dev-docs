---
slug: /reference/sdk.snapshotentryinput
title: SnapshotEntryInput variable
hide_title: true
displayed_sidebar: typescript
---

<!-- Do not edit this file. It is automatically generated by API Documenter. -->

# SnapshotEntryInput variable

**Signature:**

```typescript
SnapshotEntryInput: z.ZodObject<
  {
    address: z.ZodUnion<
      [
        z.ZodType<string, z.ZodTypeDef, string>,
        z.ZodType<
          `0x${string}`,
          z.ZodTypeDef,
          `${string}.eth` | `${string}.cb.id`
        >,
      ]
    >;
    maxClaimable: z.ZodDefault<
      z.ZodDefault<
        z.ZodUnion<
          [
            z.ZodEffects<
              z.ZodUnion<[z.ZodString, z.ZodNumber]>,
              string,
              string | number
            >,
            z.ZodLiteral<"unlimited">,
          ]
        >
      >
    >;
    price: z.ZodOptional<
      z.ZodDefault<
        z.ZodUnion<
          [
            z.ZodEffects<
              z.ZodUnion<[z.ZodString, z.ZodNumber]>,
              string,
              string | number
            >,
            z.ZodLiteral<"unlimited">,
          ]
        >
      >
    >;
    currencyAddress: z.ZodOptional<
      z.ZodDefault<
        z.ZodUnion<
          [
            z.ZodType<string, z.ZodTypeDef, string>,
            z.ZodType<
              `0x${string}`,
              z.ZodTypeDef,
              `${string}.eth` | `${string}.cb.id`
            >,
          ]
        >
      >
    >;
  },
  "strip",
  z.ZodTypeAny,
  {
    address: string;
    maxClaimable: string;
    price?: string | undefined;
    currencyAddress?: string | undefined;
  },
  {
    address: string;
    maxClaimable?: string | number | undefined;
    price?: string | number | undefined;
    currencyAddress?: string | undefined;
  }
>;
```