# Prometheus Redis Metrics Exporter
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
我们只是在redis exporter的基础上添加了用的的新内容，原有redis的内容没有直接删除，但不表示todis也会支持，我门只是用了相应dashboard用到的基本内容。
有其他要求可发起pull request或issues。

