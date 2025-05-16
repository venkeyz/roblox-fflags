---
title: Rendering
order: 0
---

### Metal
added by @pixelyloaf
> [!IMPORTANT]
> **MacOS only**
```json
{
    "FFlagDebugGraphicsPreferMetal": "True"
}
```
### Vulkan
added by @pixelyloaf
> [!CAUTION]
> **Visual Bugs & Crashes**
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferVulkan": "True"
}
```
### OpenGL
added by @pixelyloaf
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferOpenGL": "True"
}
```
### Direct X 10
added by @pixelyloaf
```json
{
    "FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### Direct X 11
added by @pixelyloaf
```json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```