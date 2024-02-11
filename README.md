HTTP Service for Networking Labs
================================

A simple HTTP service for networking labs. The service uses [Nginx][Nginx].

[Nginx]: http://nginx.org/

Basic Usage
-----------

Specify user names and passwords in [`htpasswd`][AuthFile] file.

[AuthFile]: https://nginx.org/en/docs/http/ngx_http_auth_basic_module.html#auth_basic_user_file

Start the service:

```sh
docker compose up --detach
```

Print logs:

```sh
docker compose logs
```

Stop the service:

```sh
docker compose down
```

Testing
-------

Send a request:

```sh
curl --location http://localhost
curl --location --user alice:pass1 http://localhost/private
```
