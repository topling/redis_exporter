# Prometheus Todis Metrics Exporter
Prometheus exporter for Todis metrics.

## Building and running the exporter

### Build and run locally

```sh
git clone https://github.com/topling/todis_exporter.git
cd todis_exporter
go build .
./todis_exporter --version
```

说明：
我们只是在 redis exporter 的基础上添加了用的的新内容，原有 redis 的内容没有直接删除，但不表示 todis 也会支持，我们只是用了相应 dashboard 用到的基本内容。
有其他要求可发起pull request或issues。

