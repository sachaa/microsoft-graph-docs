﻿# androidForWorkGmailEasConfiguration resource type

> **Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change. Use of these APIs in production applications is not supported.

> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.

By providing configurations in this profile you can instruct the Gmail email client on Android For Work devices to communicate with an Exchange server and get email, contacts, calendar, tasks, and notes. Furthermore, you can also specify how much email to sync and how often the device should sync.

Inherits from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md)

## Methods
|Method|Return Type|Description|
|---|---|---|
|[List androidForWorkGmailEasConfigurations](../api/intune_deviceconfig_androidforworkgmaileasconfiguration_list.md)|[androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md) collection|List properties and relationships of the [androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md) objects.|
|[Get androidForWorkGmailEasConfiguration](../api/intune_deviceconfig_androidforworkgmaileasconfiguration_get.md)|[androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md)|Read properties and relationships of the [androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md) object.|
|[Create androidForWorkGmailEasConfiguration](../api/intune_deviceconfig_androidforworkgmaileasconfiguration_create.md)|[androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md)|Create a new [androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md) object.|
|[Delete androidForWorkGmailEasConfiguration](../api/intune_deviceconfig_androidforworkgmaileasconfiguration_delete.md)|None|Deletes a [androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md).|
|[Update androidForWorkGmailEasConfiguration](../api/intune_deviceconfig_androidforworkgmaileasconfiguration_update.md)|[androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md)|Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune_deviceconfig_androidforworkgmaileasconfiguration.md) object.|
|[List deviceConfigurationGroupAssignments](../api/intune_deviceconfig_deviceconfigurationgroupassignment_list.md)|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|List properties and relationships of the [deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) objects.|
|[List deviceConfigurationDeviceStatuses](../api/intune_deviceconfig_deviceconfigurationdevicestatus_list.md)|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) objects.|
|[List deviceConfigurationUserStatuses](../api/intune_deviceconfig_deviceconfigurationuserstatus_list.md)|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) objects.|
|[Get deviceConfigurationDeviceOverview](../api/intune_deviceconfig_deviceconfigurationdeviceoverview_get.md)|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md) object.|
|[Get deviceConfigurationUserOverview](../api/intune_deviceconfig_deviceconfigurationuseroverview_get.md)|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Read properties and relationships of the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.|
|[List settingStateDeviceSummaries](../api/intune_deviceconfig_settingstatedevicesummary_list.md)|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|List properties and relationships of the [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) objects.|
|[Get androidForWorkCertificateProfileBase](../api/intune_deviceconfig_androidforworkcertificateprofilebase_get.md)|[androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|Read properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md) object.|

## Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignmentStatus|String|Read-only. DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignmentProgress|String|Read-only. DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|assignmentErrorMessage|String|Read-only. DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|authenticationMethod|String|Authentication method for Exchange ActiveSync. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md) Possible values are: `usernameAndPassword`, `certificate`.|
|durationOfEmailToSync|String|Duration of time email should be synced to. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md) Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.|
|emailAddressSource|String|Email attribute that is picked from AAD and injected into this profile before installing on the device. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md) Possible values are: `userPrincipalName`, `primarySmtpAddress`.|
|hostName|String|Exchange location (URL) that the mail app connects to. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md)|
|requireSsl|Boolean|Indicates whether or not to use SSL. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md)|
|usernameSource|String|Username attribute that is picked from AAD and injected into this profile before installing on the device. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md) Possible values are: `username`, `userPrincipalName`.|

## Relationships
|Relationship|Type|Description|
|---|---|---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune_deviceconfig_deviceconfigurationgroupassignment.md) collection|The list of group assignments for the device configuration profile. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection|Device configuration installation stauts by device. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection|Device configuration installation stauts by user. Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection|Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune_deviceconfig_androidforworkcertificateprofilebase.md)|Identity certificate. Inherited from [androidForWorkEasEmailProfileBase](../resources/intune_deviceconfig_androidforworkeasemailprofilebase.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkGmailEasConfiguration"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "assignmentStatus": "String",
  "assignmentProgress": "String",
  "assignmentErrorMessage": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "authenticationMethod": "String",
  "durationOfEmailToSync": "String",
  "emailAddressSource": "String",
  "hostName": "String",
  "requireSsl": true,
  "usernameSource": "String"
}
```



