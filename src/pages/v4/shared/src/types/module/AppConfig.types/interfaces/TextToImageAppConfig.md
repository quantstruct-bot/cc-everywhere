# Interface: TextToImageAppConfig

## Extends

- [`BaseAppConfig`](../../../DesignConfig.types/interfaces/BaseAppConfig.md)

## Properties

| Property | Type | Description | Inherited from |
| ------ | ------ | ------ | ------ |
| `callbacks?` | [`Callbacks`](../../../Callbacks.types/interfaces/Callbacks.md) | - | [`BaseAppConfig`](../../../DesignConfig.types/interfaces/BaseAppConfig.md).`callbacks` |
| `analyticsData?` | [`BaseAnalyticsData`](../../../AppConfig.types/type-aliases/BaseAnalyticsData.md) | Analytics data that can be provided by the host app | [`BaseAppConfig`](../../../DesignConfig.types/interfaces/BaseAppConfig.md).`analyticsData` |
| `headerBarColorTheme?` | [`ColorTheme`](../../../AppConfig.types/enumerations/ColorTheme.md) | Theming options for the TextToImage Editor header bar. **Default** `ColorTheme.LIGHT` | - |
| `editorTitle?` | `string` | Property to configure the title | - |
| `promptText?` | `string` | - | - |
| `imageDimensions?` | [`ImageDimensions`](../../../Asset.types/type-aliases/ImageDimensions.md) | The dimensions of the image that the user can generate. If provided, the user will be restricted to generating images of the specified dimensions. | - |
| `imageStyleReference?` | [`Asset`](../../../Asset.types/type-aliases/Asset.md) | Asset to be passed as style reference for generating images | - |
| `imageCompositionReference?` | [`Asset`](../../../Asset.types/type-aliases/Asset.md) | Asset to be passed as composition reference for generating images | - |
| `appVersion?` | [`TextToImageAppVersion`](../enumerations/TextToImageAppVersion.md) | Specifies the version of the Generate Image experience to be enabled. This setting allows the selection between the older and the newer interface version. When set to the latest version (V2), users will get access to the updated interface and features. By default, the older experience (V1) is displayed. Enabling the latest version introduces the following key features: - **Enhanced User Interface:** Redesigned with a new Carousel and Grid view. - **Community Wall:** An endless collection of generated images with prompts that users can select from to kickstart their image generation journey. - **Fast Mode:** Images can be generated faster with lesser details, great for simple topics, backgrounds, most illustrations, and close portraits. - **Improved Prompt Bar:** Includes prompt suggestions for a better user experience. - **Rich Previews:** Provides a more interactive and engaging preview experience. - And more! **Default** `V1` | - |
| `editDropdownOptions?` | [`EditDropdownOptionConfig`](EditDropdownOptionConfig.md)[] | Options to be passed for Edit dropdown. NOTE: This property is supported only in the new Generate Image experience. **Default** `[ { option: EditFurtherIntent.APPLY_ADJUSTMENT }, { option: EditFurtherIntent.APPLY_EFFECTS }, { option: EditFurtherIntent.REMOVE_BACKGROUND }, { option: EditFurtherIntent.REMOVE_OBJECT }, { option: EditFurtherIntent.INSERT_OBJECT } ]` | - |
| `publishConfig?` | [`PublishConfig`](PublishConfig.md) | Config to be set for Publish action. NOTE: This property is supported only in the new Generate Image experience. **Default** `{ * id: "saveToHostApp", * label: "Save" * }` | - |
| `thumbnailOptions?` | [`ThumbnailOption`](../enumerations/ThumbnailOption.md)[] | Options passed to be displayed on the thumbnail. NOTE: This property is supported only in the new Generate Image experience. **Default** `[ ThumbnailOption.EDIT_DROPDOWN, ThumbnailOption.RICH_PREVIEW ]` | - |
| `fastModeConfig?` | [`FastModeConfig`](FastModeConfig.md) | Configuration for enabling or disabling fast mode in the Text to Image module. NOTE: This property is supported only in the new Generate Image experience and when FAST_MODE is set to true in featureConfig. **Default** `{ * defaultFastModeState: 'off' * }` | - |
| `featureConfig?` | `Partial`<`Record`<[`TextToImageFeature`](../enumerations/TextToImageFeature.md), `boolean`\>\> | Configuration for enabling or disabling specific features in the Text to Image module. NOTE: This property is supported only in the new Generate Image experience. **Default** `{ * [TextToImageFeatureType.COMMUNITY_WALL]: false, * [TextToImageFeatureType.FAST_MODE]: false * }` | - |
| `communityWallConfig?` | [`CommunityWallConfig`](CommunityWallConfig.md) | - | - |
