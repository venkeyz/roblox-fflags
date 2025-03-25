# roblox-fflags

![GitHub commit activity](https://img.shields.io/github/commit-activity/t/pixelyloaf/roblox-fflags?authorFilter=pixelyloaf&style=for-the-badge&logo=github) 

![GitHub commit activity](https://img.shields.io/github/commit-activity/t/pixelyloaf/roblox-fflags?authorFilter=venkeyz&style=plastic)

build status ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/pixelyloaf/roblox-fflags/retype-action.yml?style=for-the-badge)


list of fflags on roblox i've seen sorted into folders

if you want it here i'm working on it (mostly one section every commit)

## Rendering

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
### Direct X 11
```json
{
    "FFlagDebugGraphicsPreferD3D11": "True"
}
```

## Lighting

### Voxel Lighting (Phase 1)
```json
{
    "DFFlagDebugRenderForceTechnologyVoxel": "True"
}
```
### Shadowmap Lighting (Phase 2)
```json
{
    "FFlagDebugForceFutureIsBrightPhase2": "True"
}
```
### Future Lighting (Phase 3)
```json
{
    "FFlagDebugForceFutureIsBrightPhase3": "True"
}
```
### Unified Lighting
```json
{
    "FFlagRnderUnifiedLighting12": "True",
    "FFlagUnifedLightingBetaFeature": "True"
}
```
### Unified Lighting Blendzone
```json
{
    "FIntUnifiedLightingBlendZone": "500"
}
```

## Graphics

### Set how many pixels to render
```json
{
    "DFIntDebugDynamicRenderKiloPixels": "1"
}
```
### Disable Highlights
```json
{
    "DFFlagRenderHighlightMangerPrepare": "True"
}
```
### Enable DRS
```json
{
    "FFlagRenderDynamicResolutionScale12": "True"
}
```
### Move Pre-Render Phase [~25 Performance Boost]
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
```json
{
    "FIntGrassMovementReducedMotionFactor": "999"
}
```
```json
{
    "FIntGrassMovementReducedMotionFactor": "0"
}
```
### Enable Highlight Outlines on any Rendering API
```json
{
    "FFlagHighlightOutlinesOnMobile": "True"
}
```
### No Bloom/Clouds

```json
{
    "FFlagRenderNoLowFrmBloom": "False"
}
```
### Render Occlusion Culling

```json
{
    "DFFlagUseVisBugCheks": "True",
    "FFlagEnableVisBugChecks27": "True",
    "FFlagVisBugChecksThreadYield": "True",
    "FIntEnableVisBugChecksHundredthPercent27": "100"
}
```
### Increased Particles on low graphics

```json
{
    "FFlagDebugDeterministicParticles": "True"
}
```
### Makes stuff slightly brighter
```json
{
    "FFlagRenderFixFog": "True"
}
```
### HyperThreading
```json
{
    "FFlagDebugCheckRenderThreading": "True",
    "FFlagRenderDebugCheckThreading2": True
}
```
### Maximum Threads
```json
{
    "FIntRuntimeMaxNumOfThreads": "2400"
}
```
### Minimum Threads
```json
{
    "FIntTaskSchedularThreadMin": "3"
}
```
### Smoother Terrain
```json
{
    "FFlagDebugRenderingSetDeterministic": "True"
}
```
### Force Graphics Quality Level
```json
{
    "FIntRomarkStartWithGraphicsQualityLevel": "1"
}
```
### Disable Player Shadows
```json
{
    "FIntRenderShadowIntensity": "0"
}
```
### Preserve rendering quality with display setting
```json
{
    "DFFlagDisableDPIScale": "True"
}
```
### Low Graphics Quality w/ Max Render Distance/FRM Quality Levels
> [!TIP]
> **1-6 Are low graphics, Above 6 are high graphics. Like the 1-21 graphics slider**
```json
{
    "DFIntDebugFRMQualityLevelOverride": "1"
}
```

### FRM 21 Graphics Quality Slider
```json
{
    "FFlagCommitToGraphicsQualityFix": "True",
    "FFlagFixGraphicsQuality": "True"
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
### Disables fade in and out animation every light update
```json
{
    "FIntRenderLocalLightFadeInMs": "0"
}
```
### Make avatars shiny
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
```json
{
    "FFlagDisablePostFx": "True"
}
```
### Pause Voxelizer/Disable Baked Shadows
```json
{
    "DFFlagDebugPauseVoxelizer": "True"
}
```
### Grey sky
> [!IMPORTANT]
> **Only applies to games with the default skybox**
```json
{
    "FFlagDebugSkyGray": "True"
}
```
### Force LOD on Meshes
```json
{
    "DFIntCSGLevelOfDetailSwitchingDistance": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL12": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL23": "0",
    "DFIntCSGLevelOfDetailSwitchingDistanceL34": "0"
}
```
### Lighting Attenuation
```json
{
    "FFlagNewLightAttenuation": "True"
}
```
### Enable GPULightCulling
> [!TIP]
> **Combine with LightingAttenuation for better vision**
```json
{
    "FFlagFastGPULightCulling3": "True"
}
```
### Enable CPULightCulling
```json
{
    "FFlagDebugForceFSMCPULightCulling": "True"
}
```
### Frame buffer
> [!TIP]
> **0 makes white screen 1-3 makes other players have laggy movement, 4 is stable has better performance than 10 and less input lag**
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### Low Quality Terrain Textures
> [!TIP]
> **4 for less quality 16, 32, 64 for higher quality**
```json
{
    "FIntTerrainArraySliceSize": "4"
}
```
### Force Texture Quality
> [!TIP]
> **Set any value from 0-3**
```json
{
    "DFFlagTextureQualityOverrideEnabled": "True",
    "DFIntTextureQualityOverride": "3"
}
```
### Lower Quality Textures
```json
{
    "DFIntPerformanceControlTextureQualityBestUtility": "-1"
}
```
### No avatar textures
```json
{
    "DFIntTextureCompositorActiveJobs": "0"
}
```
### Texture Manager
> [!TIP]
> 1-4 Blurry, 5-7 low quality also removes studs, 8 Removes almost everything
```json
{
    "FIntDebugTextureManagerSkipMips": "8"
}
```
### Remove Grass
```json
{
    "FIntFRMMinGrassDistance": "0",
    "FIntFRMMaxGrassDistance": "0",
    "FIntRenderGrassDetailStrands": "0",
}
```
### Force MSAA
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
> [!IMPORTANT]
> **Future & ShadowMap only**
```json
{
    "FIntRenderShadowmapBias": "75"
}
```
### Limits number of animations being played
> [!TIP]
> **0 removes most player animations, 1-5 removes the walk animation after jumping**
```json
{
    "DFIntMaxActiveAnimationTracks": "0"
}
```

## Quality of Life

### DO NOT DISTURB/Disable Notifications
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Disable VC
> [!NOTE]
> Setting this to `True` will not do anything
```json
{
    "DFFlagVoiceChat4": "False"
}
```
### Remove translated supported message on join
> [!NOTE]
> `"Roblox automatically translates supported languages in chat."`
```json
{
    "FFlagChatTranslationEnableSystemMessage": false
}
```

### Allows you to customize which languages are available for the chat translation feature
> [!IMPORTANT]
> English cannot be removed.


```json
{
    "FStringChatTranslationEnabledLocales": "es_es,fr_fr,pt_br,de_de,it_it,ja_jp,ko_kr,id_id,tr_tr,zh_cn,zh_tw,th_th,pl_pl,vi_vn,ru_ru,"
}
```
### Remove long recommended section in homepage
```json
{
    "FIntGameGridFlexFeedItemTileNumPerFeed": "0"
}
```
### Disable Captures Keybind
```json
{
    "FFlagEnableCapturesHotkeyExperiment_v4": "False"
}
```
### Reduced Avatar Item Particle in FP
```json
{
    "FFlagUserHideCharacterParticlesInFirstPerson": "True"
}
```
### FPS Unlocker in Roblox Menu Settings
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### Unlimited FPS Unlocker
```json
{
    "FFlagTaskSchedulerLimitTargetFpsTo2402": "False",
    "DFIntTaskSchedulerTargetFps": "9999"
}
```
### GUI Hiding Toggles
```json
{
    "FFlagUserShowGuiHideToggles": "True",
    "GuiHidingApiSupport2": "True"
}
```
### Hide GUIs
> [!IMPORTANT]
> Replace "ID" with any group ID that you are in.

| Key combination   | Action                                                                    |
| ----------------- | ------------------------------------------------------------------------- |
| Ctrl + Shift + B  | Toggles GUIs in 3D space (BillboardGuis, SurfaceGuis, etc)                |
| Ctrl + Shift + C  | Toggles game-defined ScreenGuis                                           |
| Ctrl + Shift + G  | Toggles Roblox CoreGuis                                                   |
| Ctrl + Shift + N  | Toggles player names, and other BillboardGuis that show up above a player |
```json
{
    "DFIntCanHideGuiGroupId": "ID"
}
```
### Remove layered clothing related for searching in lua app catalog
```json
{
    "FStringAXCategories": "ClassicShirts.ClassicTShirts.ClassicPants"
}
```
### Disable Fullscreen Title Bar
```json
{
    "FIntFullscreenTitleBarTriggerDelayMillis": "3600000"
}
```
### Stuttery Animation Fix
```json
{
    "DFIntTimestepAbiterThresholdCFLThou": "300"
}
```
### Disable In-game Advertisements
```json
{
    "FFlagAdServiceEnabled": "False"
}
```
### Disable Telemetry
```json
{
    "FFlagDebugDisableTelemetryEphemeralCounter": "True",
    "FFlagDebugDisableTelemetryEphemeralStat": "True",
    "FFlagDebugDisableTelemetryEventIngest": "True",
    "FFlagDebugDisableTelemetryPoint": "True",
    "FFlagDebugDisableTelemetryV2Counter": "True",
    "FFlagDebugDisableTelemetryV2Event": "True",
    "FFlagDebugDisableTelemetryV2Stat": "True"
}
```
### Surf the web inside of Roblox
> [!IMPORTANT]
> **Click the Beta Badge of the 13+ badge to open the webview browser.**
```json
{
    "FFlagTopBarUseNewBadge": "True",
    "FStringTopBarBadgeLearnMoreLink": "https://udm14.com/",
    "FStringVoiceBetaBadgeLearnMoreLink": "https://udm14.com/"
}
```
### MTU
==- :icon-question: View Full Documentation
> [!TIP]
> **Identify the Current MTU**
> - **Windows**: Open Command Prompt and type 'netsh interface ipv4 show subinterfaces`.
> - **Linux**: Use 'ifconfig' or 'ip link show' to find the current MTU of your network interface.

> [!TIP]
> **Determine the Optimal MTU**
> - **Ping Test**: Use the `ping` command with the `-f` flaf (to avoid fragmentation) and the `l` (or `s` on Linux) flag to set the global packet size.
> - **Example for Windows**:
> ```bash
> ping roblox.com -f -l 1472
> ```
> - **Example for Linux**:
> ```bash
> ping -s 1472 -M do roblox.com
> ```
> - Start with a packet size of 1472 bytes, then reduce by 10-12 bytes if needed until you find the largest size that doesn't fragment. Add 28 bytes to this number to get the optimal MTU.
===
```json
{
    "DFIntConnectionMTUSize": "MTU_HERE"
}
```
### No Internet Disconnect
> [!NOTE]
> **You will still be kicked but the message will not show.**
```json
{
    "DFFlagDebugDisableTimeoutDisconnect: "True"
}
```
### Adjust Default Timeout Time
> [!TIP]
> **1 second = 1000**


```json
{
    "DFIntDefaultTimeoutTimeMs": "10000"
}
```
### Quick Game Launch
> [!CAUTION]
> **This can cause some bugs**
```json
{
    "FFlagEnableQuickGameLaunch": "True"
}
```
### Increased Asset Preloading Count
==- :icon-question: View Full Documentation
> [!NOTE]
> **Increasing the maximum limit of preloaded assets from 100 to infinite allows games you've already played to load much faster by instantly accessing previously loaded assets.**

> [!IMPORTANT]
> **For this to be effective, the game must have been fully loaded at least once, perferably with the entire map cached.**

> [!TIP]
> **If a game has a "Skip Loading" button, it's recommended to use it. These games typically include a countdown timer that, after reaching zero, merely confirms that all assets are loaded.**
===

```json
{
    "DFIntNumAssestsMaxToPreload": "9999999",
    "DFIntAssetPreloading": "9999999"
}
```
### Disable In-Gmae Purchases
```json
{
    "DFlagOrder66": "True"
}
```
### Disable Chat
```json
{
    "FFlagDebugForceChatDisabled": "True"
}
```
### Disable Dynamic Heads Animations
```json
{
    "DFIntAnimationLodFacsDistanceMin": "0",
    "DFIntAnimationLodFacsDistanceMax": "0",
    "DFIntAnimationLodFacsVisibilityDenominator": "0"
}
```
### Automatically unmuts your mic on join (VC)
```json
{
    "FFlagDebugDefaultChannelStartMuted": "False"
}
```
### opt-out Experience Language
> [!NOTE]
> **Removes the Experience Language option in settings**
```json
{
    "FIntV1MenuLanguageSelectionFeaturePerMillageRollout": "0"
}
```
### Lets you change the zoom out limit
> [!IMPORTANT]
> **Only applies to games that has not changed the default zoom limit**
```json
{
    "FIntCameraMaxZoomDistance": "9999"
}
```
### Exclusive Fullscreen
> [!TIP]
> Alt + Delete
```json
{
    "FFlagHandleAltEnterFullscreenManually": "False"
}
```
### Change Age Rating Learn More Link
```json
{
    "FStringExperienceGuidelinesExplainedPageUrl": "https://udm14.com/"
}
```
### Rename Party 2 Roblox Chat
```json
{
    "FFlagAppChatRebrandStringUpdates": "False"
}
```
### 5 decimal digits limit for camera sensitivity
> [!NOTE]
> basically like idk 8 months ago roblox added a 3 decimal digits limit, some people that I know used those extra digits
```json
{
    "FFlagFixSensitivityTextPrecision": "False"
}
```

## UI+Visuals

### Revert Debug Menu UI Change
```json
{
    "FFlagImproveMicroprofilerReadability": "False"
}
```
### Red Font/Highlight Font
```json
{
    "FStringDebugHighlightSpecificFont": "rbxasset://fonts/families/BuilderSans.json"
}
```
### Voicechat Mute Toggles
![example](https://github.com/user-attachments/assets/186d3b58-5560-4ea7-ba6f-cc62f8ab5351)
```json
{
    "FFlagMuteTogglesEnableIXP": "False"
}
```
### Mini Webview
```json
{
    "FFlagWebViewProtocol": "False"
}
```
### THICK Healthbar
```json
{
    "FFlagUpdateHealthBar": "True"
}
```
### Remove Parental Controls Tab
```json
{
    "FFlagLuaAppsEnableParentalControlsTab": "False"
}
```
### Legacy Search
```json
{
    "FFlagAXSearchLandingPageIXPEnabled4": "False"
}
```
### Disable Profile Picture Customization
```json
{
    "FFlagAXDefaultAvatarToShopEnabled3": "False"
}
```
```json
{
    "FFlagEnableNewChatTabExperiment5": "False
}
```
### Disable Toast Notifications
```json
{
    "FFlagToastNotificationsProtocolEnabled2": "False"
}
```
### Rename Communications to Voice Enabled
```json
{
    "FFlagGameDetailsDecoupledCommunication": "False"
}
```
### Break Reduced Motion V4

![image](https://github.com/user-attachments/assets/cfdc9732-084e-4c09-bc43-8039a3bf0d89)
```json
{
    "FFlagFixReducedMotionStuckIGM2": "False"
}
```
### Revert "Charts" back to Discovery
```json
{
    "FFlagLuaChartsPageRenameIXP": "False"
}
```
### Disable Sidebar
```json
{
    "FFlagEnableNavBarLabels3": "False"
}
```
### V2 Menu
```json
{
    "FIntNewInGameMenuPercentRollout3": "100",
    "FFlagEnableInGameMenuControls": "False",
    "FFlagDisableDisableNewIGMinDUA": "True",
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlagEnableInGameMenuSongbirdABTest": "False"
}
```
### Custom Disconnect Message
```json
{
    "FFlagReconnectDisabled": "True",
    "FStringReconnectDisabledReason": "disconnection jumpscare"
}
```
### Display FPS
```json
{
    "FFlagDebugDisplayFPS": "True"
}
```
### Verified Badge
> [!NOTE]
> Cliensided only
```json
{
    "FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified Badge on everyone
> [!NOTE]
> Clientsided only
```json
{
    "FFlagOverridePlayerVerifiedBadge": "True"
}
```
### Applies cool colours to stuff
```json
{
    "FFlagDebugDisplayUnthemedInstances": "True"
}
```
### Revert new invite menu
```json
{
    "FFlagEnableNewInviteMenuIXP2": "False"
}
```
### Revert spacing on errors
```json
{
    "FFlagErrorPromptResizesHeight": "False"
}
```
### Remove Disconnect Blur/Loading Blur
```json
{
    "FIntRobloxGuiBlurIntensity": "0"
}
```
### Disable New Chat Translation Settings
```json
{
    "FFlagChatTranslationSettingEnabled3": "False"
}
```
### New Camera Mode
```json
{
    "FFlagNewCameraControls": "True"
}
```
### Custom MicroProfile Scale
```json
{
    "DFIntMicroProfilerDpiScaleOverride": "100"
}
```
### Disable New MicroProfiler/Debug UIs
```json
{
    "FFlagImproveMicroprofilerReadability": "False"
}
```
### Adjust Scroll Speed
```json
{
    "FIntScrollWheelDeltaAmount": "140"
}
```
### Set Custom Kick Message Length
```json
{
    "FIntMaxKickMessageLength": "1"
}
```
### Disable New Blue Theme
```json
{
    "FFlagLuaAppUseUIBloxColorPalettes1": "False",
    "FFlagLuaAppEnableFoundationColors7": "False"
}
```
### Enable New Settings Layout
```json
{
    "FFlagInExperienceMenuReorderFirstVariant2": "True"
}
```
### No Transparency V4 Menu **(2023)**
```json
{
    "FStringInGameMenuModernizationStickyBarForcedUserIds": "UserID"
}
```
### Subscriptions Page
```json
{
    "FFlagLuaDevSubsEnabled": "True"
}
```
### Overlay that shows what you type
```json
{
    "FFlagDebugTextBoxServiceShowOverlay": "True"
}
```
### Amount of lines to show at once for above
```json
{
    "DFIntTextBoxServiceHistorySize": "1"
}
```
### Hides gui
```json
{
    "DFIntTextBoxServiceHistorySize": "1"
}
```
### Dont Render UI
```json
{
    "FFlagDebugDontRenderUI": "True"
}
```
### Don't Render Screen GUIs
```json
{
    "FFlagDebugDontRenderScreenGui": "True"
}
```
### Disable Autocomplete
```json
{
    "FFlagEnableCommandAutocomplete": "False"
}
```
### Break Top Bar Menu
```json
{
    "FStringNewInGameMenuForceds": "UserID",
    "FFlagEnableInGameMenuChrome": "True"
}
```
### Break Collectible Icon
```json
{
    "FFlagDisplayCollectiblesIcon": "False"
}
```
### Disable Bubble Chat
```json
{
    "FFlagEnableBubbleChatFromChatService": "False"
}
```
### Disable Avatar Chat
```json
{
    "FFlagAvatarChatServiceEnabled3": "False"
}
```
### Remove VC beta badge
```json
{
    "FFlagVoiceBetaBadge": "False",
    "FFlagTopBarUseNewBadge": "False",
    "FFlagBetaBadgeLearnMoreLinkFormview": "False",
    "FFlagControlBetaBadgeWithGuac": "False",
    "FStringVoiceBetaBadgeLearnMoreLink": "null"
}
```
### VR Controller transparency
```json
{
    "FIntVRTouchControllerTransparency": "0"
}
```
### Disable VR Collision Fade
```json
{
    "FFlagViewCollisionFadeToBlackInVR": "False"
}
```
### Limit Videos Playing
```json
{
    "DFIntVideoMaxNumberOfVideosPlayting": "0"
}
```
### Disable DSA Reporting In-Game

```json
{
    "FFlagDSAIllegalContentReporting2": "False"
}
```
### Desktop App Dev Tools
> [!IMPORTANT]
> Only works on web view windows like profiles, Ctrl + Shift + I
```json
{
    "FFlagDebugEnableNewWebView2DevTool": "True"
}
```
### Enable Events Tab/Change Events Tab URL
```json
{
    "FFlagPlatformEventEnabled2": "True",
    "FStringPlatformEventUrl": "https://udm14.com/" 
}
```
### Better Trackpad Scrolling
```json
{
    "FFlagBetterTrackpadScroling": "True"
}
```
### Reset Character instead of Respawn in Experience Menu
```json
{
    "FFlagInExperienceMenuResetButtonTextToRespawn": "False"
}
```

## Audio

### Allows you to change voice chat distance
> [!NOTE]
> **Default: [Min 7 Max 80]**
```json
{
    "DFIntVoiceChatRollOffMinDistance": "7",
    "DFIntVoiceChatRollOffMaxDistance": "80"
}
```
### Sounds use physical velocity and become distorted
> [!NOTE]
> **<2017 Audio**
```json
{
    "FFlagSoundsUsePhysicalVelocity": "True"
}
```
### Audio Occlusion
```json
{
    "FFlagDebugEnableDirectAudioOcclusion2": "True"
}
```
### Limit audios that are being played
```json
{
    "DFIntMaxLoadableAudioChannelCount": "1"
}
```
### Mess with voice chat volume
[!NOTE]
> **Default: 1000**
```json
{
    "DFIntVoiceChatVolumeThousandths" "100000"
}
```
### No sounds
```json
{
    "FFlagDebugRomarkMockingAudioDevices": "True"
}
```

## Abusive

### Teleport All Ragdolls/Unanchored to 0, 0, 0
> [!NOTE]
> Clientsided
```json
{
    "DFIntGameNetLocalSpaceMaxSendIndex": "1000"
}
```
### No Knockback/Ragdoll
```json
{
    "DFIntGameNetLocalSpaceMaxSendIndex": "100000",
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Tool desync
```json
{
    "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
}
```
### Desync FFlag
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
```json
{
    "FFlagRemapAnimationR6ToR15Rig": "True"
}
```
### Weird leg movement
```json
{
    "DFFlagAnimatorPostProcessIK": "True"
}
```
### Random High Jumps
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### Drunk
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```
### No animations
> [!NOTE]
> **Stops the game trying to replicate your animations in the server. You dont have animations in the server but you do for your client**
```json
{
    "DFIntReplicatorAnimationTrackLmiitPerAnimator": "-1"
}
```
### Delayed Animations
```json
{
    "FFlagProcessAnimationLooped": "False"
}
```
### Stick unanchored parts to you
> [!TIP]
> **- = up, + = down**
```json
{
    "DFIntSolidFloorPercentForceApplication": "-1000",
    "DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```
### Max Raycast Distance
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
> [!NOTE]
> **A.k.a does not let you load games**
```json
{
    "DFIntDataSenderRate": "-1"
}
```
### Disable Touch Events
```json
{
    "DFIntTouchSenderMaxBandwidthBps": "-1"
}
```
### Improved Syncing
```json
{
    "DFIntS2PhysicsSenderRate": "10000"
}
```
### Clientsided Invisible
```json
{
    "FIntParallelDynamicPartsFastClusterBatchSize": "-1"
}
```
### Invisible 1
> [!NOTE]
> Stops the physics on your character from sending to the server so your character doesnt move for the server. You can move on your client.
```json
{
    "DFIntS2PhysicsSenderRate": "-30"
}
```
### Invisible 2
> [!NOTE]
> Locks your character's position on the server to (0, 0, 0), having the side effect of turning you invisible. This only affects the server and other clients, not you. server-sided things that rely on your position, like clicking to get tools, will not function. In some games these can be abusable.
```json
{
    "DFIntGameNetPVHeaderTranslationZeroCutOffExponent": "10"
}
```
### Warp
```json
{
    "DFIntMaxMissedWorldStepsRemembered": "1000"
}
```
### Noclip 1
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
```json
{
    "DFIntPhysicsDecompForceUpgradeVersion": "1500"
}
```
### Wallglide
```json
{
    "DFIntMaximumUnstickForceInGs": "-10"
}
```
### Network Ownership
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
```json
{
    "DFIntPhysicsImprovedCyclicExecutiveThrottleThresholdTenth": "0"
}
```
### Fake lag
```json
{
    "DFIntS2PhysicSenderRate": "1"
}
```

# Abusive Visuals

### Semi Fullbright
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
```json
{
    "FFlagDebugAvtarChatVisualization": "True",
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlagEnableIngameMenuChrome": "False",
    "FFlagEnableInGameMenuSongbirdABTest": "False"
}
```
### Humanoid Outline
> [!NOTE]
> **Draws an outline around every part and every humanoid**
```json
{
    "DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```
### fflag above but more complex
> [!NOTE]
> **Draws an outline around every body part**
```json
{
    "DFFlagDebugDrawBvhNodes": "True"
}
```
### Buggy ZPlane Camera
```json
{
    "FIntCameraFarZPlane": "1"
}
```
### Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's as non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
    "FFlagDebugHumanoidRendering": "True"
}
```

## Misc

### spammed
```json
{
    "FIntDebugTextElongationFactor": "6785"
}
```
### break everything
```json
{
    "DFIntHttpRbxApiClientPerMinuteRequestLimit": "60",
    "DFIntHttpRbxApiJobFrequencyInSeconds": "60",
    "DFIntHttpRbxApiMaxBudgetMultiplier": "2",
    "DFIntHttpRbxApiMaxRetryBudgetPerMinute": "60",
    "DFIntHttpRbxApiMaxRetryCount": "3",
    "DFIntHttpRbxApiMaxRetryQueueSize": "1000",
    "DFIntHttpRbxApiMaxSyncRetries": "3",
    "DFIntHttpRbxApiPerMinuteRequestLimit": "60",
    "DFIntHttpRbxApiSameUrlRequestLimit": "30",
    "DFIntHttpRbxApiServiceDecaySeconds": "300",
    "DFIntHttpRbxApiMaxThrottledQueue": "500"
}
```
### Stop the Chinese from spying on you
```json
{
    "FStringTencentAuthPath": "null"
}
```
### omg i cant believe roblox is that dumb to do this...
```json
{
    "FIntPhysicsGridHierarchyLowestLevelInitBinCount": "199999999",
    "FIntPhysicsGridHierarchyLowestLevelInitBinCount": "100000000",
    "FIntPhysicsSolverCollisionPoolBucketSize": "2147483647",
    "FIntPhysicsSolverCollisionPoolBucketSizeWorldModel": "2147483647"
}
```
### Crash Roblox 1
```json
{
    "DFIntTimestepArbiterThresholdCFLThou": "0"
}
```
### Crash Roblox 2
```json
{
    "DFFlagVideoCaptureServiceEnabled": "False"
}
```
### Increase Ping
```json
{
    "DFIntDataSenderMaxBandwithBps": "150"
}
```

# :icon-gear: Debug

### Replace all Decals with a Test Image

```json
{
    "FFlagDebugTestImageDrawItem": "True"
}
```
### Shows the state of a flag
```json
{
    "FStringDebugShowFlagState": "FLAG_HERE"
}
```
#### e.g
```json
{
    "FStringDebugShowFlagState": "DFIntTaskSchedulerTargetFps, ChannelName"
}
```
### Show Outlined Chunks
```json
{
    "FFlagDebugLightGridShowChunks": "True"
}
```
### Show Outlined Chunks that are being interacted
```json
{
    "DFFlagDebugEnableStreamingSolverVisualization": "True"
}
```
### Prevents Remote Events from running

```json
{
    "DFIntRemoteEventSingleInvocationSizeLimit": "1"
}
```
### Show All Error Strings
```json
{
    "FFlagDebugEnableErrorStringTesting": "True"
}
```
### logs stuff in dev console
```json
{
    "FStringDebugLuaLogLevel": "verbose",
    "FStringDebugLuaLogPattern": "ExpChat/mountClientApp"
}
```
### Octree Validation
```json
{
    "FFlagDebugEnableOctreeValidation": "True"
}
```
### Self Explanatory 1
```json
{
    "DFFlagDebugPrintDataPingBreakDown": "True"
}
```
### Self Explanatory 2
```json
{
    "DFFlagDebugAudioLogging": "True"
}
```
### Duplicate of Above
```json
{
    "DFFlagDebugAudioLogging2": "True"
}
```
### Self Explanatory 3
```json
{
    "FFlagTrackerLodControllerDebugUI": "True"
}
```
### Self Explanatory 4
> [!NOTE]
> **Disable Drag Detectors**
```json
{
    "FFlagDragDetectors1": "False"
}
```
### Self Explanatory 5
> [!NOTE]
> **Disable CTM Climbing**
```json
{
    "FFlagUserClickToMoveSupportAgentCanClimb2": "False"
}
```
### Self Explanatory 6
> [!NOTE]
> **Disable Feedback Button in ESC**
```json
{
    "FFlagDisableFeedbackSoothsayerCheck": "False"
}
```
### Self Explanatory 7

```json
{
    "FFlagRenamePassesAndGeatToSubscriptionsAndPasses": "False"
}
```
### Self Explanitory 8
```json
{
    "DFFlagDebugSimulateHangAtStartup": "True"
}
```
### Self Explanatory 9
```json
{
    "DFFlagDebugSimulateHangAtShutdown": "True"
}
```
### Self Explanatory 10
> [!NOTE]
> **LDL Program Stats**
```json
{
    "DFFlagDebugSimLDLProgramPrintBuildStats": "True",
    "DFFlagDebugSimLDLProgramPrintExecStats": "True"
}
```
### Self Explanatory 11
```json
{
    "FFlagDebugCountSimBodyAllocations": "True"
}
```
### Self Explanatory 12
```json
{
    "FIntNewDevConsoleMaxLogCount": "2147483647"
}
```
### Self Explanatory 13
```json
{
    "FFlagDebugAlwaysDisplayRenderStats": "True"
}
```
### Self Explanatory 14
###### set to 0 for the super fps boost trust it works
```json
{
    "FIntRenderMaxShadowAtlasUsageBeforeDownscale": "650"
}
```
### Self Explanatory 15
> [!NOTE]
> Allows you to edit the DataModel Patch
```json
{
    "FFlagDataModelPatcherForceLocal": "True"
}
```

## Experimental

### Voicechat in Party
> [!NOTE]
> Person(s) you want to party with **must** have both of these to be disabled otherwise they won't be able to hear you/speak
```json
{
    "FFlagEnablePartyVoiceOnlyForUnfilteredThreads": "False",
    "FFlagEnablePartyVoiceOnlyForEligibleUsers": "False"
}
```
### Experience Menu Refactror
```json
{
    "FFlagDebugRefactorInExpGameSettings": "True"
}
```
### Enable Multi Try On
```json
{
    "FFlagAXEnableMultiTryOnUI": "True"
}
```
### Enable Posts
```json
{
    "FFlagCapturesPostEnabledForAll_v4": "True"
}
```
### New Experience Menu
```json
{
    "FFlagRefactorInExpGameSettings": "True"
}
```
### Enable First Time User Experience for Chrome UI
```json
{
    "FFlagEnableChromeFTUX": "True"
}
```
### Chrome UI Topbar Removal
```json
{
    "FFlagEnableInGameMenuChromeABTest4": "False",
    "FFlaEnableInGameMenuSongbirdABTest4": "False"
}
```
### Hide playerlist close button on Chrome UI
```json
{
    "FFlagDisablePlayerListDisplayCloseBtn": "True"
}
```
### Self Explanatory i think
```json
{
    "FFlagChromeUsePreferredTransparency": "True"
}
```
### Ragdoll Death Type

> [!IMPORTANT]
> **Studio Only**

```json
{
    "DFStringDefaultAvatarDeathType": "Ragdoll"
}
```
### crash__()

> [!IMPORTANT]
> **Studio Only**
```json
{
    "FFlagDebugCrashEnabled": "False"
}
```