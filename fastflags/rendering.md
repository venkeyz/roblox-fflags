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
> **causes visual bugs and crashes**
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferVulkan": "True"
}
```
### DirectX 10
```json
{
    "FFlagDebugGraphicsPreferD3D11FL10": "True"
}
```
### DirectX 11
```json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```
### OpenGL
```json
{
    "FFlagDebugGraphicsDisableDirect3D11": "True",
    "FFlagDebugGraphicsPreferOpenGL": "True"
}
```