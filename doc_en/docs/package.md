# Packaging & Building

To build a project using the Magenta Realtime 2 plugin and create a package, you must configure the Asset Manager so that AI model assets are included in the package.

## How to Configure Asset Manager

Add an element to "Project Settings > Game > Asset Manager > Primary Asset Types to Scan" and set the following values:  
Alternatively, "PrimaryAssetLabel" is configured at Index=1 by default, so editing that element is also OK.

1. Set **Primary Asset Types** to `PrimaryAssetLabel`.
2. Set **Asset Base Class** to `PrimaryAssetLabel`.
3. Turn off **Is Editor Only**.
4. Add an element to **Specific Assets** and specify `MagentaRealtime2_AudioGeneration_FP16`.

!!! Info "When using [32-bit float](../performance/#switching-fp16-fp32)"
    Specify `MagentaRealtime2_AudioGeneration_**FP32**` instead of `MagentaRealtime2_AudioGeneration_**FP16**`.

!!! Info "When using [Prefill State from Audio](../state/#setting-state-from-audio)"
    Add another element to **Specific Assets** and specify `MagentaRealtime2_Prefill`.
