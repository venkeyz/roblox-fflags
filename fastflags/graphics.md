---
title: Graphics
icon: device-desktop
order: -3
---
### Pause voxelizer/Disable baked shadows
```json
{
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Grey sky
> [!IMPORTANT]
> only applies to games with the default skybox
```json
{
    "FFlagDebugSkyGray": "True"
}
```
### Lower quality textures
```json
{
    "DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### Frame buffer
> [!TIP]
> 0 makes white screen | 1-3 makes other players have laggy movement | 4 is stable with better performance than 10
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### Force graphics quality level
```json
{
    "FIntRomarkStartWithGraphicsQualityLevel": "1"
}
```
### Low render distance
```json
{
    "DFIntDebugRestrictGCDistance": "1"
}
```
### Limit light updates
```json
{
    "FIntRenderLocalLightUpdateMax": "8",
    "FIntRenderLocalLightUpdatesMin": "6"
}
```