# Class: `abstract` FeatureFlagService

Abstract class for feature flag services

## Extended by

- [`LocalFeatureFlagService`](../../LocalFeatureFlagService/classes/LocalFeatureFlagService.md)

## Constructors

### new FeatureFlagService()

```ts
new FeatureFlagService(): FeatureFlagService
```

#### Returns

[`FeatureFlagService`](FeatureFlagService.md)

## Methods

### getFeatureFlagsParams()

```ts
getFeatureFlagsParams(
   intent, 
   isFirstParty, 
   clientId, 
   analyticsClientId?): URLSearchParams
```

Generates URL-encoded feature flag parameters for a specific client and intent

#### Parameters

| Parameter | Type |
| ------ | ------ |
| `intent` | [`ActionIntent`](../../../../../shared/src/types/ActionIntent.types/type-aliases/ActionIntent.md) |
| `isFirstParty` | `boolean` |
| `clientId` | `string` |
| `analyticsClientId`? | `string` |

#### Returns

`URLSearchParams`
