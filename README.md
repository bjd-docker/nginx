# Nginx image

## Usage

### docker-compose

```yaml
version: '3'

services:
  nginx:
    image: 'bjouhaud/nginx'
    hostname: 'nginx'
    ports:
      - '80:80'
    volumes:
      - '.:/app:ro'
    environment:
      VIRTUAL_HOST: '***.localhost'
```
