# eth2-metrics

This is an aggregate of all the different Eth2-client metrics, and related useful dashboards.

Some client sources used different job name, template, data-sources, etc. This aggregate aims to standardize those.

Conventions:
- `${DS_PROMETHEUS}` is used for `datasource`, referring to `Prometheus` by default, via the `templating` `current` value.
  This enables configuration, while having a (very) common default to rely on with provisioning.
- `beacon` is used as job-name in dashboards to refer to beacon nodes.
- `validator` is used as job-name in dashboards to refer to standalone validator clients.
- `eth2client` is used as label to identify a particual client. Expected values: `prysm`, `lighthouse`, `teku`, `nimbus`, `lodestar`, `trinity`
