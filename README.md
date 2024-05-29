待办：
1. 关于token持久化
因为还不太清楚pinia持久化的使用，所以没有添加，而是手动添加在localStorage中
2. 本地缓存一个时间戳，以验证登录是否过期
3. 登录接口返回值中的money在后台是数字类型，而在store中我设置的是字符串类型
4. 持久化登录（自动登录）


沟通：
<!-- 1. register接口缺少一个返回值：id -->
<!-- 2. 登录接口返回值中的money是什么意思 -->
3. 登录接口还得返回一个标识身份的数据以区分展示用户端还是管理端页面
<!-- 4. 需要添加一个接口用于通过id获取用户信息，如头像、昵称、邮箱等 -->

bug：
1. 一个邮箱可以绑定注册多个账号
2. 注册按钮可以多次点击

思考：
1. 关于检查登录过期时间并自动登录：在localStorage中设置过期时间戳，判断代码写在stores/index.js中

备忘：
1. 本地缓存数据：token、登录时间戳、id、昵称、邮箱、头像