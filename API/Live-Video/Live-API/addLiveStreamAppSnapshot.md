# addLiveStreamAppSnapshot


## 描述
添加APP直播截图配置

## 请求方式
POST

## 请求地址
https://live.jdcloud-api.com/v1/snapshotApps:template


## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**appName**|String|True| |直播流所属应用名称|
|**publishDomain**|String|True| |您的推流加速域名|
|**template**|String|True| |截图模版|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|ruquestId|


## 返回码
|返回码|描述|
|---|---|
|**400**|Invalid parameter|
|**401**|Authentication failed|
|**404**|Not found|
|**503**|Service unavailable|
|**200**|OK|
|**500**|Internal server error|
