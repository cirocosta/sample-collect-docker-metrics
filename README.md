<h1 align="center">Sample Docker daemon metrics collection</h1>

<h5 align="center">
  <a href="https://ops.tips/gists/how-to-collect-docker-daemon-metrics/">
    How to collect Docker Daemon Metrics
  </a>
</h5>

<br />
<br />


An example of how to make use of [Prometheus](https://prometheus.io/), [Grafana](https://grafana.com/) and [Docker daemon metrics](https://docs.docker.com/config/thirdparty/prometheus/) to graph Docker daemon statistics.

![Illustration of the Docker metrics collection](https://ops.tips/gists/-/images/docker-daemon-grafana-metrics.png)

### Usage

```sh
make  run                 # builds grafana and prometheus 
                          # images and initializes all three containers 
                          # that forms the infra (grafana, prometheus and 
                          # node_exporter).  

make  update-dashboards   # updates the list of json files that represent
                          # the dashboards configured in Grafana.

```

<br />
<br />

### More

See:

- [How to Collect Docker Daemon Metrics]().
- [Initializing Grafana with preconfigured dashboards](https://ops.tips/blog/initialize-grafana-with-preconfigured-dashboards/).
