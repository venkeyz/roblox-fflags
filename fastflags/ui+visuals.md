---
title: UI+Visuals
icon: versions
order: 4
---
### Custom disconnect message
> [!NOTE]
> if you want to change the text edit disconnection jumpscare
```json
{
    "FFlagReconnectDisabled": "True",
    "FStringReconnectDisabledReason": "disconnection jumpscare"
}
```
### Disable blue theme
```json
{
    "FFlagLuaAppUseUIBloxColorPalettes1": "False",
    "FFlagLuaAppEnableFoundationColors7": "False"
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
### Verified badge
> [!NOTE]
> clientsided
```json
{
    "FStringWhitelistVerifiedUserId": "UserID"
}
```
### Verified badge on everyone
> [!NOTE]
> also clientsided
```json
{
    "FFlagOverridePlayerVerifiedBadge": "True"
}
```
### Disable sidebar
```json
{
    "FFlagLuaAppChartsPageRenameIXP": "False"
}
```
### Desktop DevTools
> [!IMPORTANT]
> only works on webview
```json
{
    "FFlagDebugEnableNewWebView2DevTool": "True"
}
```
### Revert Respawn text
```json
{
    "FFlagInExperienceMenuResetButtonTextToRespawn": "False"
}
```