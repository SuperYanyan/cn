# attachDiskToVmInstanceByDiskId


## 描述
云硬盘挂载至虚拟机

## 请求方式
PUT

## 请求地址
https://jdfusion.jdcloud-api.com/v1/regions/{regionId}/disk_disks/{id}:attach

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**id**|String|True| |云硬盘 ID|
|**regionId**|String|True| |地域ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**attach**|AttachDataDisk|True| |云硬盘挂载至虚拟机|
|**authorization**|String|True| |获取方式请参考签名算法指导文档|
|**x-jdcloud-date**|String|True| |获取方式请参考签名算法指导文档|
|**x-jdcloud-fusion-cloudid**|String|True| |云注册信息ID|
|**x-jdcloud-nonce**|String|True| |获取方式请参考签名算法指导文档|

### AttachDataDisk
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**deleteWithInstance**|Boolean|False| |释放实例时，该云盘是否随实例一起释放。默认值：False|
|**instanceId**|String|True| |虚拟机 id|

## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|请求ID|
|**result**|Result| |

### Result
|名称|类型|描述|
|---|---|---|
|**task**|ResourceTFInfo| |
### ResourceTFInfo
|名称|类型|描述|
|---|---|---|
|**body**|String|请求体|
|**cloudId**|String|cloud ID|
|**createdTime**|String|创建时间|
|**provider**|String|cloud provider|
|**result**|String|执行结果|
|**status**|String|状态|
|**updateTime**|String|更新时间|
|**userId**|String|user ID|
|**uuid**|String|uuid|

## 返回码
|返回码|描述|
|---|---|
|**201**|CREATED|
