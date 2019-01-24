# Ansible Role: prometheus-mosquitto-exporter

An Ansible role that installs [Prometheus Mosquitto Exporter](https://github.com/sapcc/mosquitto-exporter) on Ubuntu|Debian

## Requirements

All needed packages will be installed with this role.

## Dependencies

- UnderGreen.prometheus-exporters-common

## Example Playbook

```yaml
- hosts: mosquitto-exporters
  roles:
    - role: agricool.prometheus-mosquitto-exporter
      prometheus_mosquitto_exporter_version: 0.5.0
      prometheus_mosquitto_exporter_config_flags:
        'web.listen-address': '0.0.0.0:9100'
        'log.level': 'info'
```

## License

GPLv2
