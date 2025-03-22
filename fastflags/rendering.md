---
title: Rendering
icon: cpu
order: 0
---

### Metal
> [!IMPORTANT]
> **MacOS only**
```json
{
    "FFlagDebugGraphicsPreferMetal": "True"
}
```
### Vulkan
> [!CAUTION]
> **Visual Bugs & Crashes**
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferVulkan": "True"
}
```
### OpenGL
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferOpenGL": "True"
}
```
### Direct X 10
```json
{
    "FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### Direc tX 11
```json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```