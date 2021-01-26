# sphinx-exporter

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/sphinx-exporter/status.svg)](https://drone.osshelp.ru/ansible/sphinx-exporter)

Ansible role that installs and configures [sphinx-exporter](https://github.com/iamseth/sphinx_exporter).

## Usage (example)

```yaml
    - role: sphinx-exporter
```

Configure only:

```yaml
    - role: redis-exporter
      sphinx_exporter_setup: configure
      spinx_exporter_params: "-sphinx.host localhost -sphinx.port 9312"
```

## Available parameters

Global settings and defaults.

| Param | Description |
| -------- | -------- |
| sphinx_exporter_version | Which exporter version to install. The value will be used in binary download url formation. Available releases could be found [here](https://github.com/iamseth/sphinx_exporter/releases). Default version is 0.0.2. |
| sphinx_exporter_setup | Setup mode. See [OSSHelp KB article](https://oss.help/kb4895). Default value is full. |
| sphinx_exporter_params | Exporter starting params. Default value is "-sphinx.host localhost -sphinx.port 9312". |

## Useful links

- [Official documentation](https://github.com/iamseth/sphinx_exporter))
- [Our article](https://oss.help/kb2211)

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
