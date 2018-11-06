Prometheusbeat example manifests. 

Example configuration for prometheus-operator

```
  remoteWrite:
  - url: "http://prometheusbeat:8080/prometheus"
    writelabelConfigs:
    - sourceLabels:
      - "__name__"
      regex:         lts.+
      action:        keep
```
