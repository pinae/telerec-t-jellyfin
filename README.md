# telerec-t-jellyfin
Telerec’t Role for Jellyfin

Add this role with:

```bash
git submodule add git@github.com:pinae/telerec-t-jellyfin.git roles/jellyfin
```

## Configuration

Please change the passwords! A block like this lives in `group_vars/all.yml`:

```yaml
jellyfin:
  name: jellyfin
  directory: "{{ docker_dir }}/jellyfin"
  domain: "jellyfin.example.com"
  # url_path_prefix: "/jellyfin"
  movies_dir: "{{ data_dir }}/movies"
  tvseries_dir: "{{ data_dir }}/tv"
  traefik: true
  external: false
  watchtower: true
  autoheal: true
```
