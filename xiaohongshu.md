
# 小红书接口

接口说明
* 账号注册请联系v:feilang235，添加好友请备注:api
* 所有接口均有权限验证，每个用户有唯一的token
* 所有接口均返回json格式，其中 code 为 0 时表示响应成功，
* 会增加调用次数。否则不会影响调用量。
* 所有接口响应都很快，timeout 时间建议在5s内
* 如需其他接口和数据，可定制开发
* 内部使用，侵权联系删除
* 所有接口没有特殊说明请求方式均为 GET


## 获取笔记详情
```
path：
/xhs/api/app/note

params：	
token	验证码   
note_id 笔记id

response：
返回值与小红书接口一样，对数据进行透传，请按照小红书页面对照理解意思
```

## 获取笔记评论列表
```
path：
/xhs/api/app/note/comment

params：
token	验证码
note_id 笔记id
end_id  默认为0，列表最后用户id作为下一页翻页参数

response：
返回值与小红书接口一样，对数据进行透传，请按照小红书页面对照理解意思
```

## 获取用户个人页信息
```
path：
/xhs/api/app/user

params：
token	验证码
user_id 用户id

response：
返回值与小红书接口一样，对数据进行透传，请按照小红书页面对照理解意思
```

## 获取用户笔记列表
```
path：
/xhs/api/app/user/note

params：
token	验证码
user_id 用户id
page    默认为1，翻页参数

response：
返回值与小红书接口一样，对数据进行透传，请按照小红书页面对照理解意思
```

## 搜索笔记列表
```
path：
/xhs/api/app/search/note

params：
token	验证码
type 排序类型（hot=最热 time=最新 general=综合，默认：general）
sort 图文类型（videos=视频 notes=图文 all=不限，默认：all）
page    默认为1，翻页参数

response：
返回值与小红书接口一样，对数据进行透传，请按照小红书页面对照理解意思
```