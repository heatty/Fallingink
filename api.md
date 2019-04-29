# 接口文档

## 1 用户模块 user
### 1.1 登录 login
接口：user/login
方式：POST
响应：

### 1.2 随机匹配 connect\_by\_random
接口：users/connect\_by\_random
方式：GET
参数：uid，timestamp，token
响应：
json
{
    code: 0,
    message: 'success',
    data: {}
}


### 1.3 定向匹配 connect\_by\_id
接口：users/connect\_by\_id
方式：GET
参数：uid，timestamp，token，user\_id
响应：
json
{
    code: 0,
    message: 'success',
    data: {}
}


### 1.4 解除匹配 disconnect
接口：users/disconnect
方式：GET
参数：uid，timestamp，token
响应：
json
{
    code: 0,
    message: 'success'
}


### 1.5 更新用户信息 update
接口：users/update
方式：POST
参数：uid，timestamp，token，name，face，sex
响应：
json
{
    code: 0,
    message: 'success'
}


### 1.6 获取用户信息 user
接口：users/user
方式：GET
参数：uid，timestamp，token，user\_id
响应：
json
{
    code: 0,
    message: 'success',
    data: {}
}



### 1.7 获取通知信息接口 show\_notification
接口：users/show\_notification
方式：GET
参数：uid，timestamp，token
响应：
json
{
    code: 0,
    message: 'success',
    data: []
}



## 2. 日记模块 notes
### 2.1 发布日记 publish
接口：notes/publish
方式：POST
参数：uid，timestamp，token，title，content，images，latitude，mode
响应：
json
{
    code: 0,
    message: 'success'
}


### 2.2 删除日记 delete
接口：notes/delete
方式：GET
参数：uid，timestamp，token，note\_id
响应：
json
{
    code: 0,
    message: 'success'
}


### 2.3 获取日记列表 list
接口：notes/list
方式：GET
参数：uid，timestamp，token
响应：
json
{
    code: 0,
    message: 'success',
    data: {
        user: [],
        note
    }
}


### 2.4 编辑日记 update
接口：notes/update
方式：POST
参数：uid，timestamp，token，note\_id，title，content，images，mode
响应：
json
{
    code: 0,
    message: 'success'
}



## 3 工具模块 utils
### 3.1 请求上传图片接口 qiniu\_token
接口：utils/qiniu\_token
方式：GET
参数：uid，timestamp，token，filename
响应：
json
{
    code: 0,
    message: 'success',
    data: {}
}

