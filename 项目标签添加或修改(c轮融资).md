# 项目标签添加(c轮融资)

## 1. API 描述：添加项目融资标签信息


## 2. 调用方法

> post /api/project-tag-save

## 2. 请求参数

当传入id是修改信息，不传入id添加信息

参数 | 解释 | 类型 | 是否必须 | 示例数据
:---:|:---|:---:|:---:|:---
id | 项目tag的id号 | int | 否 | 
projectId | 项目id号 | int | 是 |
tagName | 标签名称 | string | 是 |



## 3. 响应状态

状态码 | 说明
:---:|:---
200 | 操作成功


## 4. 响应数据

参数 | 解释 | 类型 | 是否必须 | 示例数据
:---:|:---|:---:|:---:|:---



## 5. 示例
{url}/api/project-tag-save

### 请求数据：

```json
{
	"projectId":1,
	"tagName":"c轮融资"
}
```


### 响应结果：

遍历data中的content显示

projectStatus：项目状态  1-未接触、2-初次接触、3-NDA、4-TS、5-DD
projectImportant：项目重要性：1-低  2-中  3-高


```json
{
    "code": 200,
    "msg": "success",
    "data": {
        "id": 3,
        "projectId": 1,
        "tagName": "c轮融资",
        "createdAt": null,
        "updatedAt": null
    }
}
```
