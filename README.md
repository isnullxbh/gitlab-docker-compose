# gitlab-docker-compose

Install GitLab with Docker Compose

## Prerequisites

Create a directory for GitLab configs, logs and data:

```shell
sudo mkdir -p /srv/gitlab
```

If you decide to use a different path, make changes to the [env](.env) file.

## Compose

1. Edit parameters in the [env](.env) file.
2. Run `docker compose up --detach`.

## Author

Oleg E. Vorobiov <isnullxbh@gmail.com>
