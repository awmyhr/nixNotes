# TICK stack

From the InfluxData site: the TICK stack is "The Platform for Time-Series Data".
It covers the collection, storage, visualization, processing, monitring, and
alerting of time-series data.

The TICK stack is comprised of:

    - Telegraf [https://github.com/influxdata/telegraf]
    - InfluxDB [https://github.com/influxdata/influxdb]
    - Chronograf [https://github.com/influxdata/chronograf]
    - Kapacitor [https://github.com/influxdata/kapacitor]

The entire stack is open source developed primarily by InfluxData[https://influxdata.com].

## Main Components

### Telegraf

This is the agent for collecting and reporting metrics.

### InfluxDB

This is the database for the metrics.

### Chronograf

This is the front-end.

### Kapacitor

This provides monitring & alerting.

## Extras

### Grafana

In the past I have used Grafana as a front-end to InfluxDB, and it can still be
used as part of the TICK stack.

## Architecture

### Docker

Official Docker images are available.

https://hub.docker.com/_/telegraf/
https://hub.docker.com/_/influxdb/
https://hub.docker.com/_/chronograf/
https://hub.docker.com/_/kapacitor/


