---
title: UI+Visuals
icon: versions
order: 4
---
### Custom disconnect message
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