# 会员地址添加(user.address.add)

## 用户相关API

### 

* 系统参数

| *字段* | *标题* | *数据类型* | *验证条件* | *示例值* | *默认值* | *详细说明* |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| method | API的方法名 | string | required | trade.get | null | 标识请求的是哪个API |
| timestamp | 请求时间 | unix时间戳 | required , numeric , > time()-300 | 1440596821 | null | 标识API请求的发起时间，如果超时300秒则拒绝请求 |
| format | 返回数据格式 | string | required | json | json | 返回数据是json格式的，目前只支持json |
| v | 版本号 | string | required | v1 | null | 标识该接口的版本 |
| sign_type | 签名方式 | string | required | MD5 | null | 标识签名算法 |
| sign | 签名 | string | required | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA | null | 数据签名，32位长度16进制数字 |


* 业务参数

| *字段* | *标题* | *数据类型* | *验证条件* | *示例值* | *默认值* | *详细说明* |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| user_id |  | int | required |  |  | 用户ID必填 |
| addr_id |  | int |  |  |  | 商品ID必填 |
| area |  | string | required |  |  | 地区 |
| addr |  | string | required |  |  | 地址 |
| zip |  | string |  |  |  | 邮编 |
| name |  | string | required |  |  | 会员名称 |
| mobile |  | string |  |  |  | 电话 |
| def_addr |  | bool |  |  |  | 是否是设为默认 |


*返回内容示例

```



```

