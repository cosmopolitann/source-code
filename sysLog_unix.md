### 										Syslog-unix

1.文件名

```go
syslog_unix.go
```



2.路径

```go
log 包
```



3.阅读

```go
package syslog

import (
	"errors"
	"net"
)

// unixSyslog opens a connection to the syslog daemon running on the
// local machine using a Unix domain socket.

 unixSyslog  在本地机器使用一个 Unix 进程 套接字  去连接 正在运行的  syslog 进程。

 

func unixSyslog() (conn serverConn, err error) {
	logTypes := []string{"unixgram", "unix"}
	logPaths := []string{"/dev/log", "/var/run/syslog", "/var/run/log"}
	for _, network := range logTypes {
		for _, path := range logPaths {
			conn, err := net.Dial(network, path)
			if err == nil {
				return &netConn{conn: conn, local: true}, nil
			}
		}
	}
	return nil, errors.New("Unix syslog delivery error")
}


```

