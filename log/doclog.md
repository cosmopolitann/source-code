### 											Log

1.文件名

```go
log
doc.go

```



2.Path

```go
log包下的 doc.go
```



```go
// Copyright 2012 The Go Authors. All rights reserved.
// Use of this source code is governed by a BSD-style
// license that can be found in the LICENSE file.

GO 作者 在 2012 获得 版权证书   保留所有版权权利。
使用源码将受到BSD-style 约束
版权许可证可在 许可文件中找到.
```





```go
// Package syslog provides a simple interface to the system log
// service. It can send messages to the syslog daemon using UNIX
// domain sockets, UDP or TCP.
//
// Only one call to Dial is necessary. On write failures,
// the syslog client will attempt to reconnect to the server
// and write again.
//
// The syslog package is frozen and is not accepting new features.
// Some external packages provide more functionality. See:
//
//   https://godoc.org/?q=syslog
syslog 包 为 系统日志服务 提供了一个简单的接口。
它能使用 UNIX 领域套接字 UDP 或者 Tcp  发送 信息 给日志进程。

仅仅通过拨打一个电话就可以了，如果写入失败
这是syslog  客户端 就会 允许重新连接 服务器 并 再次写入。

这个syslog 包 是被冻结的，不接受新的功能。
一些外部的包 提供更多的函数。 看这些：

 https://godoc.org/?q=syslog


```

