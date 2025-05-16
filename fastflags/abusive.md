---
title: Abusive
icon: alert-fill
order: -7
---
> [!CAUTION]
> FastFlags are not bannable by Roblox, but abusing them can get you banned from certain games.

### Teleport All Ragdolls/Unanchored to 0, 0, 0
added by @pixelyloaf
> [!NOTE]
> Clientsided
```json
{
    "DFIntGameNetLocalSpaceMaxSendIndex": "1000"
}
```
### No Knockback/Ragdoll
added by @pixelyloaf
```json
{
    "DFIntGameNetLocalSpaceMaxSendIndex": "100000",
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Tool desync
added by @pixelyloaf
```json
{
    "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
}
```
### Desync FFlag
added by @venkeyz
```json
{
    "DFFlagPhysicsSkipNonRealTimeHumanoidForceCalc2": "False",
    "DFIntS2PhysicsSenderRate": "3",
    "DFIntTaskSchedularTargetFps": "5588562",
    "FFlagGameBasicSettingsFramerateCap5": "False",
    "FFlagTaskSchedularLimitTargetFpsTo2402": "False"
}
```
### Remap R6 to R15 Rigs/Weird Movement
added by @pixelyloaf
```json
{
    "FFlagRemapAnimationR6ToR15Rig": "True"
}
```
### Weird leg movement
added by @pixelyloaf
```json
{
    "DFFlagAnimatorPostProcessIK": "True"
}
```
### Random High Jumps
added by @pixelyloaf
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### Drunk
added by @pixelyloaf
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### No animations
added by @pixelyloaf
> [!NOTE]
> **Stops the game trying to replicate your animations in the server. You dont have animations in the server but you do for your client**
```json
{
    "DFIntReplicatorAnimationTrackLmiitPerAnimator": "-1"
}
```
### Delayed Animations
added by @pixelyloaf
```json
{
    "FFlagProcessAnimationLooped": "False"
}
```
### Stick unanchored parts to you
added by @pixelyloaf
> [!TIP]
> **- = up, + = down**
```json
{
    "DFIntSolidFloorPercentForceApplication": "-1000",
    "DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```
### Max Raycast Distance
added by @pixelyloaf
> [!NOTE]
> **Raycasting is the use of intersection tests to solve problems in Roblox. The most common use of raycasting is to determine the first object intersected by a ray. This is done by casting a virtual ray from a certain point in a direction and determing the first surface it intersected with.**

> [!TIP]
> **Break legs collision from 2 to -inf, kinda break camera on values over 3 noclip cam on 3**
```json
{
    "DFIntRaycastMaxDistance": "3"
}
```
### Change DataSender Rate
added by @pixelyloaf
> [!NOTE]
> **A.k.a does not let you load games**
```json
{
    "DFIntDataSenderRate": "-1"
}
```
### Disable Touch Events
added by @pixelyloaf
```json
{
    "DFIntTouchSenderMaxBandwidthBps": "-1"
}
```
### Improved Syncing
added by @pixelyloaf
```json
{
    "DFIntS2PhysicsSenderRate": "10000"
}
```
### Clientsided Invisible
added by @pixelyloaf
```json
{
    "FIntParallelDynamicPartsFastClusterBatchSize": "-1"
}
```
### Invisible 1
added by @pixelyloaf

moved by @venkeyz
> [!NOTE]
> Stops the physics on your character from sending to the server so your character doesnt move for the server. You can move on your client.
```json
{
    "DFIntS2PhysicsSenderRate": "-30"
}
```
### Invisible 2
added by @pixelyloaf

moved by @venkeyz
> [!NOTE]
> Locks your character's position on the server to (0, 0, 0), having the side effect of turning you invisible. This only affects the server and other clients, not you. server-sided things that rely on your position, like clicking to get tools, will not function. In some games these can be abusable.
```json
{
    "DFIntGameNetPVHeaderTranslationZeroCutOffExponent": "10"
}
```
### Warp
added by @pixelyloaf
```json
{
    "DFIntMaxMissedWorldStepsRemembered": "1000"
}
```
### Noclip 1
added by @pixelyloaf
> [!NOTE]
> this currently looks broken to me, might not work for you (good job roblox, honestly)

> [!TIP]
> **Adjust the value so you don't fall through the ground**
```json
{
    "DFIntAssemblyExtentsExpansionStudHundredth": "-50"
}
```
### Noclip 2/Mesh Noclip
added by @pixelyloaf
```json
{
    "DFIntPhysicsDecompForceUpgradeVersion": "1500"
}
```
### Wallglide
added by @pixelyloaf
```json
{
    "DFIntMaximumUnstickForceInGs": "-10"
}
```
### Network Ownership
added by @pixelyloaf
> [!NOTE]
> better [network ownership](https://create.roblox.com/docs/physics/network-ownership) of parts

> [!CAUTION]
> **This might get you banned in some games with anticheats (Limbobbia)**
```json
{
    "DFIntMinClientSimulationRadius": "2147000000",
    "DFIntMinimalSimRadiusBuffer": "2147000000",
    "DFIntMaxClientSimulationRadius": "2147000000",
    "DFFlagDebugPhysicsSenderDoesNotShrinkSimRadius": "True",
    "FFlagDebugUseCustomSimRadius": "True"
}
```
### Drive Vehicles Slow
added by @pixelyloaf
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Fake lag
added by @pixelyloaf
```json
{
    "DFIntS2PhysicSenderRate": "1"
}
```

# Abusive Visuals

### Semi Fullbright
added by @pixelyloaf
```json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAnnenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Draws a circle under avatars
added by @pixelyloaf
```json
{
    "FFlagDebugAvtarChatVisualization": "True",
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlagEnableIngameMenuChrome": "False",
    "FFlagEnableInGameMenuSongbirdABTest": "False"
}
```
### Humanoid Outline
added by @pixelyloaf
> [!NOTE]
> **Draws an outline around every part and every humanoid**
```json
{
    "DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```
### fflag above but more complex
added by @pixelyloaf
> [!NOTE]
> **Draws an outline around every body part**
```json
{
    "DFFlagDebugDrawBvhNodes": "True"
}
```
### Buggy ZPlane Camera
added by @pixelyloaf
```json
{
    "FIntCameraFarZPlane": "1"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's as non-functioning UI too. Also adds a blue circle to your humanoid.
added by @pixelyloaf
```json
{
    "FFlagDebugHumanoidRendering": "True"
}
```
