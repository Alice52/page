## 简要描述

- 用户注册接口

!> 注意：文档的链接都要以 #/ 开头。

?> You can ignore the `package.json`

## 请求 URL

- `http://localhost:9887/api/pub/login`

## 请求方式

- POST
- application/json

## 请求示例

```json
{
  "account": "admin",
  "password": "admin"
}
```

## 参数

| 参数名   | 必选 | 类型   | 说明 |
| :------- | :--- | :----- | ---- |
| account  | 是   | string | 账号 |
| password | 是   | string | 密码 |

## 返回示例

```json
{
  "code": 0,
  "msg": "登录成功"
}
```

```json
{
  "code": 1,
  "msg": "user does not exist"
}
```

## 返回参数说明

| 参数名 | 类型   | 说明                   |
| :----- | :----- | ---------------------- |
| code   | int    | 返回码，0-正常，1-异常 |
| msg    | string | 返回消息               |
