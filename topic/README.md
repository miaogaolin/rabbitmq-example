# 发送消息

```shell
go run emit_log_topic.go "A.B.C" "hello"

go run emit_log_topic.go "D.B.C" "world"
```

# 接受消息
```shell

# 匹配所有
go run receive_logs_topic.go "#"

# 匹配部分
go run receive_logs_topic.go "D.#"
go run receive_logs_topic.go "*.B.C"
```