![WorkspaceModel](../images/workspacesMetaModel.png)

### **Node Definitions**

#### Node Label: Workspace

|Property|Description|
|----|----|
|id|system generated
|Name |


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
|Person|Workspace|MEMBER_OF
|Person|Workspace|REFERENCED
|BusinessTrend|Workspace|REFERENCED
|TechnologyTrend|Workspace|REFERENCED
|Solution|Workspace|REFERENCED
|Industry|Workspace|REFERENCED
|SubIndustry|Workspace|REFERENCED
|BusinessArea|Workspace|REFERENCED
|Attachment|Workspace|INCLUDES
|WorkspaceNote|Workspace|INCLUDES
|Person|WorkspaceNote|INCLUDES
|BusinessTrend|WorkspaceNote|INCLUDES
|TechnologyTrend|WorkspaceNote|INCLUDES
|Solution|WorkspaceNote|INCLUDES
|Industry|WorkspaceNote|INCLUDES
|SubIndustry|WorkspaceNote|INCLUDES
|BusinessArea|WorkspaceNote|INCLUDES|
|Attachment|BusinessTrend|REFERENCED|occurrence
|Attachment|TechnologyTrend|REFERENCED|occurrence
|Attachment|Industry|REFERENCED|occurrence
|Attachment|SubIndustry|REFERENCED|occurrence
|Attachment|BusinessArea|REFERENCED|occurrence


_The occurrence counter is calculated via the document upload and analytics engine_


