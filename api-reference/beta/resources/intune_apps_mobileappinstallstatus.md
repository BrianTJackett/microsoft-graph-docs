﻿# mobileAppInstallStatus resource type

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

Contains properties for the installation state of a mobile app for a device.
## Methods
|Method|Return Type|Description|
|---|---|---|
|[List mobileAppInstallStatuses](../api/intune_apps_mobileappinstallstatus_list.md)|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) collection|List properties and relationships of the [mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) objects.|
|[Get mobileAppInstallStatus](../api/intune_apps_mobileappinstallstatus_get.md)|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md)|Read properties and relationships of the [mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) object.|
|[Create mobileAppInstallStatus](../api/intune_apps_mobileappinstallstatus_create.md)|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md)|Create a new [mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) object.|
|[Delete mobileAppInstallStatus](../api/intune_apps_mobileappinstallstatus_delete.md)|None|Deletes a [mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md).|
|[Update mobileAppInstallStatus](../api/intune_apps_mobileappinstallstatus_update.md)|[mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md)|Update the properties of a [mobileAppInstallStatus](../resources/intune_apps_mobileappinstallstatus.md) object.|
|[Get mobileApp](../api/intune_apps_mobileappinstallstatus_get_mobileapp.md)|[mobileApp](../resources/intune_apps_mobileapp.md)|Get the [mobileApp](../resources/intune_apps_mobileapp.md) from the app navigation property.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity.|
|deviceName|String|Device name|
|deviceId|String|Device ID|
|lastSyncDateTime|DateTimeOffset|Last sync date time|
|mobileAppInstallStatusValue|String|The install state of the app. Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`, `notApplicable`.|
|errorCode|Int32|The error code for install failures.|
|osVersion|String|OS Version|
|osDescription|String|OS Description|
|userName|String|Device User Name|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|app|[mobileApp](../resources/intune_apps_mobileapp.md)|The navigation link to the mobile app.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallStatus"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "String (identifier)",
  "deviceName": "String",
  "deviceId": "String",
  "lastSyncDateTime": "String (timestamp)",
  "mobileAppInstallStatusValue": "String",
  "errorCode": 1024,
  "osVersion": "String",
  "osDescription": "String",
  "userName": "String"
}
```



