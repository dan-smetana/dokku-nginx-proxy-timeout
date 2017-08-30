# Dokku Nginx Proxy Timeout

Dokku plugin for setting the NGINX proxy timeout by tweaking the
proxy_connect_timeout, proxy_send_timeout, proxy_read_timeout and send_timeout
directives

## Installation

```shell
# on 0.4.x+
sudo dokku plugin:install https://github.com/danielslee/dokku-nginx-proxy-timeout.git
```

## Usage

```shell
# To set a proxy timeout, set the PROXY_TIMEOUT env var
# If you unset the variable, a default of 60s will be used
dokku config:set PROXY_TIMEOUT=300s
```

## Credits

This dokku plugin was heavily inspired by
[Zeilenwerk's Dokku Nginx Max Upload Size plugin](https://github.com/Zeilenwerk/dokku-nginx-max-upload-size).
