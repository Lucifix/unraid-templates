# Unraid templates

Unraid Community Apps template for
[Model Workshop Manager](https://github.com/Lucifix/model-workshop-manager), a
self-hosted tracker for model kits, paints and builds.

```text
ca_profile.xml                       repository profile shown in Community Apps
templates/model-workshop-manager.xml the Docker template
```

## Defaults

- **Image:** `lucifix/model-workshop-manager:latest` from Docker Hub.
- **Port:** host 8080 → container 3000.
- **Folders:** data and backups are separate folders under
  `/mnt/user/appdata/model-workshop-manager/`.
- **User:** runs as `99:100` (`--user 99:100` under _Extra Parameters_).
  Unraid creates missing appdata folders owned by `nobody:users`, so the
  image's default uid 1000 couldn't write there.

Support and bug reports go to the main project's
[Discussions](https://github.com/Lucifix/model-workshop-manager/discussions)
and [issues](https://github.com/Lucifix/model-workshop-manager/issues).
