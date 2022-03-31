# Fastapi Boilerplate

_Personal use_

## Docker
```
$ docker-compose up
```

## Installation
```
$ pip3 install -r requirements.txt
```

## Usage
```
$ uvicorn app.init:app
```

### Configuration
Configuration can be changed by setting environment variables or changing the defaults in
`app/Config.py`
```python
class Configuration(ConfigBase):
    MarketplaceAddress: str = "0x821f3361D454cc98b7555221A06Be563a7E2E0A6"
    Endpoint: str = "http://127.0.0.1:8545"
    ListingsHost: str = "redis-14992.c267.us-east-1-4.ec2.cloud.redislabs.com"
    ListingsPort: str = "14992"
    ListingsPassword: str = "xxx"
    Status: str = "dev"
```