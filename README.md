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

### Basic Prometheus Configuration

Add a block to the `scrape_configs` of your prometheus.yml config file:  

```yaml
scrape_configs:
  - job_name: todis_exporter
    static_configs:
    - targets: ['<<TODIS-EXPORTER-HOSTNAME>>:9121']
```

and adjust the host name accordingly.  

## grafana dashboard
dashboard json内容在grafana_dashboard.json中，直接导入即可。

说明：
我们只是在 redis exporter 的基础上添加了用的的新内容，原有 redis 的内容没有直接删除，但不表示 todis 也会支持，我们只是用了相应 dashboard 用到的基本内容。
有其他要求可发起 pull request 或 issues。

