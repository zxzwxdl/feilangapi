
# 饿了么接口

接口说明
* 账号注册请联系v:feilang235，添加好友请备注:api
* 所有接口均有权限验证，每个用户有唯一的token
* 所有接口均返回json格式，其中 code 为 0 时表示响应成功，
* 会增加调用次数。否则不会影响调用量。
* 所有接口响应都很快，timeout 时间建议在5s内
* 如需其他接口和数据，可定制开发
* 内部使用，侵权联系删除
* 所有接口没有特殊说明请求方式均为 GET

## 店铺详情
```
path：
/ele/shop/info

params：
token	     验证码
store_id     店铺id


response：
返回值与饿了么接口一样，对数据进行透传，请按照页面对照理解意思
```

## 店铺分类列表
```
path：
/ele/cata/shop/

params：
token	     验证码
store_id     店铺id


response：
返回值与饿了么接口一样，对数据进行透传，请按照页面对照理解意思
```

## 店铺分类列表
```
path：
/ele/cata/shop/product

params：
token	     验证码
store_id     店铺id
cate_type    分类类型
cate_id      分类id
page         翻页


response：
返回值与饿了么接口一样，对数据进行透传，请按照页面对照理解意思
```
