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

## Customization

### Custom SSH port

To set a custom SSH port:

1. Add the following line to `GITLAB_OMNIBUS_CONFIG`:

   ```yaml
   gitlab_rails['gitlab_shell_ssh_port'] = <PORT>
   ```

2. Make changes to the port mappings:

   ```
   "22:22" -> "<PORT>:22"
   ```


## Author

Oleg E. Vorobiov <isnullxbh@gmail.com>
