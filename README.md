# conda-in-action
+ First to add a new channel
```
conda config --add channels conda-forge
```
+ After that the channel should be two
```
$ conda config --show
add_anaconda_token: True
add_pip_as_python_dependency: True
aggressive_update_packages:
  - ca-certificates
  - certifi
  - openssl
allow_non_channel_urls: True
allow_softlinks: False
always_copy: False
always_softlink: False
always_yes: None
anaconda_upload: None
auto_update_conda: True
changeps1: True
channel_alias: https://conda.anaconda.org
channel_priority: True
channels:
  - conda-forge
  - defaults
client_ssl_cert: None
client_ssl_cert_key: None
clobber: False
create_default_packages: []
custom_channels:
  pkgs/main: https://repo.continuum.io
  pkgs/free: https://repo.continuum.io
  pkgs/r: https://repo.continuum.io
  pkgs/pro: https://repo.continuum.io
custom_multichannels:
  defaults: ["https://repo.continuum.io/pkgs/main", "https://repo.continuum.io/pkgs/free", "https://repo.continuum.io/pkgs/r", "https://repo.continuum.io/pkgs/pro"]
  local: []
default_channels:
  - https://repo.continuum.io/pkgs/main
  - https://repo.continuum.io/pkgs/free
  - https://repo.continuum.io/pkgs/r
  - https://repo.continuum.io/pkgs/pro
disallow: []
download_only: False
envs_dirs:
  - /home/vagrant/anaconda3/envs
  - /home/vagrant/.conda/envs
force: False
json: False
local_repodata_ttl: 1
migrated_channel_aliases: []
no_dependencies: False
non_admin_enabled: True
notify_outdated_conda: True
offline: False
override_channels_enabled: True
path_conflict: clobber
pinned_packages: []
pkgs_dirs:
  - /home/vagrant/anaconda3/pkgs
  - /home/vagrant/.conda/pkgs
proxy_servers: {}
quiet: False
remote_connect_timeout_secs: 9.15
remote_max_retries: 3
remote_read_timeout_secs: 60.0
report_errors: None
rollback_enabled: True
safety_checks: warn
shortcuts: True
show_channel_urls: None
ssl_verify: True
track_features: []
use_index_cache: False
use_pip: True
verbosity: 0
whitelist_channels: []
```

+ List all the env
```
conda env list
```

+ Create new environment for python3
```
conda create -n Python35 python=3.5 --file requirements.txt
```
