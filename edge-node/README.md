### Requirements

* *docker* v24+

### Running

```
docker compose up --attach envoy
```

### Downstream traffic

**Upstream** service implemented by [httpbin.org](https://httpbin.org/)

```bash
curl -i -H "Host: example.com" http://127.0.0.1:18000/get
```

### Clean env

```bash
docker compose down --volumes --remove-orphans
```
