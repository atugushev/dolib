# Python Digital Ocean Library

[![PyPI version](https://badge.fury.io/py/dolib.svg)](https://badge.fury.io/py/dolib)
![Supported Python Versions](https://img.shields.io/pypi/pyversions/dolib)
![Tests](https://github.com/geraxe/dolib/workflows/Tests/badge.svg)
[![Coverage](https://codecov.io/gh/geraxe/dolib/branch/master/graph/badge.svg)](https://codecov.io/gh/geraxe/dolib)

## Description


## Documentation


## Requirements

Python 3.6+

DOLib uses these awesome libraries:

* <a href="https://requests.readthedocs.io/" class="external-link" target="_blank">Requests</a> for network.
* <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a> for the data parts.

## Installation

```shell
$ pip install dolib
```

## Example

```Python
from dolib import Client

client = Client(token="60c13d47f17dbed9f7293cf8c82d18fece3439a54f88e6c52c2df07f87bd8dd9")

droplets = client.droplets.all()
volume = client.volumes.get("53cf7120-9d5b-11ea-aed1-0a58ac14d008")

client.volumes.attach(volume, droplet_id=droplets[0].id)
```


## Contributing

See the [CONTRIBUTING.md](CONTRIBUTING.md) document for details.

## Versioning

This project follows [Semantic Versioning 2.0.0](http://semver.org/spec/v2.0.0.html).

## License

This project is licensed under the terms of the MIT license.
