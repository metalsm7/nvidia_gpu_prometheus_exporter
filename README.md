NVIDIA GPU Prometheus Exporter
------------------------------

Fork of [nvidia_gpu_prometheus_exporter](https://github.com/mindprince/nvidia_gpu_prometheus_exporter).

encoder_utilization, decoder_utilization added version.

## Building

```bash
$ go get github.com/metalsm7/nvidia_gpu_prometheus_exporter
$ env CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -o /usr/local/src/ github.com/metalsm7/nvidia_gpu_prometheus_exporter
```

## Install

```bash
# download binary
$ curl -LO https://github.com/metalsm7/nvidia_gpu_prometheus_exporter/releases/download/v0.1.0-alpha/nvidia_gpu_prometheus_exporter
$ chmod +x nvidia_gpu_prometheus_exporter
$ mv nvidia_gpu_prometheus_exporter /usr/local/bin/
# regist service
$ curl https://raw.githubusercontent.com/metalsm7/nvidia_gpu_prometheus_exporter/master/systemd/nvidia_gpu_prometheus_exporter.service > /etc/systemd/system/nvidia_gpu_prometheus_exporter.service
# service start
$ systemctl daemon-reload
$ systemctl enable --now nvidia_gpu_prometheus_exporter
```