# Aircloak Analysis Example

Examples of how to use the [aircloak-tools](https://github.com/diffix/aircloak-tools) package with Diffix Explorer in a Jupyter notebook.

The notebook uses the default settings from the `aircloak-tools` package:

```python
API_KEY = os.environ["AIRCLOAK_API_KEY"]
ATTACK_SERVER_API_URL = "https://attack.aircloak.com/api"
EXPLORER_DEFAULT_URL = "http://localhost"
EXPLORER_DEFAULT_PORT = 5000
```

Note this requires the AIRCLOAK_API_KEY env variable to be set to a valid api key that has access to the example datasets on `attack.aircloak.com`.

You will also need a locally running Diffix Explorer. Using the public docker image this is:

```sh
docker run \
    -d \
    --name diffix-explorer \
    --restart unless-stopped \
    -p 5000:80 \
    diffix/explorer:20.2
```

For more detail please refer to the main [Diffix Explorer](https://github.com/diffix/explorer/) repo.