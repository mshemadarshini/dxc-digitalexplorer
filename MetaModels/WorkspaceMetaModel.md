![WorkspaceModel](../images/workspacesMetaModel.png)

### **Node Definitions**

#### Node Label: Workspace

|Property|Description|
|----|----|
|id|system generated
|Name |

#### Node Label: WorkspaceGroup

|Property|Description|
|----|----|
|id|system generated
|Name |
|Public|



#### Node Label: Workspace Note

|Property|Description|
|----|----|
|id|system generated
|text|
|workspaceID|

#### Node Label: Attachment

|Property|Description|
|----|----|
|id|system generated
|Name|
|docType|
|type|MEDIA
|uri|


#### Relationships

|Source|Destination|Name|Properties|
|----|----|----|----|
|WorkspaceGroup|Account|ASSIGNED|
|Person|WorkspaceGroup|MEMBER_OF|role
|Workspace|WorkspaceGroup|MEMBER_OF|
|Person|Workspace|REFERENCED
|BusinessTrend|Workspace|REFERENCED
|TechnologyTrend|Workspace|REFERENCED
|Solution|Workspace|REFERENCED
|Industry|Workspace|REFERENCED
|SubIndustry|Workspace|REFERENCED
|BusinessArea|Workspace|REFERENCED
|Attachment|Workspace|INCLUDES|
|WorkspaceNote|Workspace|INCLUDES|
|Person|WorkspaceNote|INCLUDES|workspaceId
|BusinessTrend|WorkspaceNote|INCLUDES|workspaceId
|TechnologyTrend|WorkspaceNote|INCLUDES|workspaceId
|Solution|WorkspaceNote|INCLUDES|workspaceId
|Industry|WorkspaceNote|INCLUDES|workspaceId
|SubIndustry|WorkspaceNote|INCLUDES|workspaceId
|BusinessArea|WorkspaceNote|INCLUDES|workspaceId
|Attachment|BusinessTrend|REFERENCED|occurrence
|Attachment|TechnologyTrend|REFERENCED|occurrence
|Attachment|Industry|REFERENCED|occurrence
|Attachment|SubIndustry|REFERENCED|occurrence
|Attachment|BusinessArea|REFERENCED|occurrence


_The occurrence counter is calculated via the document upload and analytics engine_


