---
title: Graphics
order: -3
---

### Set how many pixels to render
added by @pixelyloaf
```json
{
    "DFIntDebugDynamicRenderKiloPixels": "1"
}
```
### Disable Highlights
added by @pixelyloaf
```json
{
    "DFFlagRenderHighlightMangerPrepare": "True"
}
```
### Enable DRS
added by @pixelyloaf
```json
{
    "FFlagRenderDynamicResolutionScale12": "True"
}
```
### Move Pre-Render Phase [~25 Performance Boost]
added by @pixelyloaf
==- :icon-question: View Full Documentation
> [!IMPORTANT]
> This FastFlag moves the Pre-Render task to an off thread after all other tasks are completed. By default, Pre-Render runs first, forcing the render thread to wait until the Pre-Render process finishes before it can start rendering a frame.

> [!NOTE]
> With this FastFlag enabled, Pre-Renderer is executed while the main thread is processing the previous frame. This adjustment allows the main thread to proceed without waiting for Pre-Renderer, leading to increased framerates at the expense of some frame latency.

> [!TIP]
> This flag is most effective in CPU-bound scenarios.

> [!CAUTION]
> Enabling this FastFlag may lead to input lag & crashes
===
```json
{
    "FFLagMovePrerender": "True"
}
```
### Increased Grass Motion & No Grass Motion
added by @pixelyloaf
```json
{
    "FIntGrassMovementReducedMotionFactor": "999"
}
```
added by @pixelyloaf
```json
{
    "FIntGrassMovementReducedMotionFactor": "0"
}
```
### Enable Highlight Outlines on any Rendering API
added by @pixelyloaf
```json
{
    "FFlagHighlightOutlinesOnMobile": "True"
}
```
### No Bloom/Clouds
added by @pixelyloaf
```json
{
    "FFlagRenderNoLowFrmBloom": "False"
}
```
### Render Occlusion Culling
added by @pixelyloaf
```json
{
    "DFFlagUseVisBugCheks": "True",
    "FFlagEnableVisBugChecks27": "True",
    "FFlagVisBugChecksThreadYield": "True",
    "FIntEnableVisBugChecksHundredthPercent27": "100"
}
```
### Increased Particles on low graphics
added by @pixelyloaf
```json
{
    "FFlagDebugDeterministicParticles": "True"
}
```
### Makes stuff slightly brighter
added by @pixelyloaf
```json
{
    "FFlagRenderFixFog": "True"
}
```
### HyperThreading
added by @pixelyloaf
```json
{
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": True
}
```
### Maximum Threads
added by @pixelyloaf
```json
{
    "FIntRuntimeMaxNumOfThreads": "2400"
}
```
### Minimum Threads
added by @pixelyloaf
```json
{
    "FIntTaskSchedularThreadMin": "3"
}
```
### Smoother Terrain
added by @pixelyloaf
```json
{
    "FFlagDebugRenderingSetDeterministic": "True"
}
```
### Force Graphics Quality Level
added by @pixelyloaf
```json
{
    "FIntRomarkStartWithGraphicsQualityLevel": "1"
}
```
### Disable Player Shadows
added by @pixelyloaf
```json
{
    "FIntRenderShadowIntensity": "0"
}
```
### Preserve rendering quality with display setting
added by @pixelyloaf
```json
{
    "DFFlagDisableDPIScale": "True"
}
```
### Low Graphics Quality w/ Max Render Distance/FRM Quality Levels
added by @pixelyloaf
> [!TIP]
> **1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider**
```json
{
    "DFIntDebugFRMQualityLevelOverride": "1"
}
```

### FRM 21 Graphics Quality Slider
added by @pixelyloaf
```json
{
    "FFlagCommitToGraphicsQualityFix": "True",
    "FFlagFixGraphicsQuality": "True"
}
```
### Low render distance
added by @pixelyloaf
```json
{
    "DFIntDebugRestrictGCDistance": "1"
}
```
### Limit light updates
added by @pixelyloaf
```json
{
    "FIntRenderLocalLightUpdateMax": "8",
    "FIntRenderLocalLightUpdatesMin": "6"
}
```
### Disables fade in and out animation every light update
added by @pixelyloaf
```json
{
    "FIntRenderLocalLightFadeInMs": "0"
}
```
### Make avatars shiny
added by @pixelyloaf
==- :icon-question: View Documentation
> [!TIP]
> **Everything goes black on below <3**

> [!NOTE]
> **DFIntDebugFRMQualityLevelOverride os tjere to set your graphics to 3 bars**

> [!TIP]
> **You can change it to anything above 3**
===
```json
{
    "DFIntRenderClampRoughnessMax": "-640000000",
    "DFIntDebugFRMQualityLevelOverridge": "6"
}
```
### Disable PostFX
added by @pixelyloaf
```json
{
    "FFlagDisablePostFx": "True"
}
```
### Pause Voxelizer/Disable Baked Shadows
added by @pixelyloaf
```json
{
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Grey sky
added by @pixelyloaf
> [!IMPORTANT]
> **Only applies to games with the default skybox**
```json
{
    "FFlagDebugSkyGray": "True"
}
```
### Force LOD on Meshes
added by @pixelyloaf
```json
{
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Lighting Attenuation
added by @pixelyloaf
```json
{
    "FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
added by @pixelyloaf
> [!TIP]
> **Combine with LightingAttenuation for better vision**
```json
{
    "FFlagFastGPULightCulling3": "True"
}
```
### Enable CPULightCulling
added by @pixelyloaf
```json
{
    "FFlagDebugForceFSMCPULightCulling": "True"
}
```
### Frame buffer
added by @pixelyloaf
> [!TIP]
> **0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag**
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### Low Quality Terrain Textures
added by @pixelyloaf
> [!TIP]
> **4 for less quality 16, 32, 64 for higher quality**
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### Force Texture Quality
added by @pixelyloaf
> [!TIP]
> **Set any value from 0-3**
```json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3"
}
```
### Lower Quality Textures
added by @pixelyloaf
```json
{
    "DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### No avatar textures
added by @pixelyloaf
```json
{
    "DFIntTextureCompositorActiveJobs": "0"
}
```
### Texture Manager
added by @pixelyloaf
> [!TIP]
> 1-4 Blurry, 5-7 low quality also removes studs, 8 Removes almost everything
```json
{
    "FIntDebugTextureManagerSkipMips": "8"
}
```
### Remove Grass
added by @pixelyloaf
```json
{
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
}
```
### Force MSAA
added by @pixelyloaf
> [!IMPORTANT]
> **Values: 0, 1, 2, 4, 8**

> [!CAUTION]
> **Values over 4> will cause viewport bugs**
```json
{
    "FIntDebugForcMSAASamples": "4"
}
```
### ShadowMap Bias
added by @pixelyloaf
> [!IMPORTANT]
> **Future & ShadowMap only**
```json
{
    "FIntRenderShadowmapBias": "75"
}
```
### Limits number of animations being played
added by @pixelyloaf
> [!TIP]
> **0 removes most player animations, 1-5 removes the walk animation after jumping**
```json
{
    "DFIntMaxActiveAnimationTracks": "0"
}
```