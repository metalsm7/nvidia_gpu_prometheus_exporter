NVIDIA GPU Prometheus Exporter
------------------------------

Fork of [nvidia_gpu_prometheus_exporter](https://github.com/mindprince/nvidia_gpu_prometheus_exporter).

encoder_utilization, decoder_utilization added version.

## Building

```
$ go get github.com/metalsm7/nvidia_gpu_prometheus_exporter
$ env CGO_ENABLED=1 GOOS=linux GOARCH=amd64 go build -o /usr/local/src/ github.com/metalsm7/nvidia_gpu_prometheus_exporter
```
