# SUSTech-CS305-PROJ

## Introduction



## Functions

1. http 服务器

   - [x] 接受http请求并解读请求, 存储各种数据, 将请求发送至对应方法处理
   - [x] 多线程
   - [x] LOG 日志打印 (蓝色)
   - [ ] do_GET 主功能: 
     - [x] get favicon.ico （返回图标）
     - [ ] view
       - [x] 功能
       - [ ] 返回一个好看的html界面
     - [x] download
       - [x] 功能
   - [x] do_POST 主功能
     - [x] upload
     - [x] delete
   - [x] 接收大文件, 需要根据content-length多次执行socket.recv(...)
   - [ ] 持久连接: 一个tcp连接, 多个http请求, (并行处理?)
   - [ ] 权限管理
     - [ ] 若没有携带Authorization且没有携带合法cookie, 要求认证信息
     - [ ] 若携带了Authorization, 返回cookie, 设置cookie失效时间, 完成请求
     - [ ] 若携带了合法cookie, 更新cookie失效时间, 完成请求
   - [ ] Chunk
   - [ ] 断点续传
   - [ ] RSA 加密
2. 文件系统
   + [x] 保存(上传)文件
   + [x] 获取文件内容
   + [x] 获取文件夹内容列表
   + [x] 删除文件
   + [x] 删除文件夹, 递归删除全部内容
3. 异常捕获、处理及返回: 同时包括 ERR 日志打印和对应的 HTTP response
   + [x] 定义 HTTPStatus
   + [ ] 多场景特定异常捕获
   + [ ] 返回一个好看的异常html界面
