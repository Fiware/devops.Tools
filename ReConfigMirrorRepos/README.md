## This tool:
+ creates webhook for [ApiSpecTransformer](https://github.com/FIWARE-Ops/APISpecTransformer)
+ creates webhook for [RepoSynchronizer](https://github.com/FIWARE-Ops/RepoSynchronizer)
+ changes description of repository

## How to run
```console
$ python3 run.py --mirror <PATH_TO_MIRROR_CONFIG> ---transformer <PATH_TO_TRANSFORMER_CONFIG>
```

## How to configure
+ You should provide a valid token for GitHub with an environment variable TOKEN.
+ Sample mirror config is located [here](./config-mirror-example.json).
+ Sample transformer config is located [here](./config-transformer-example.json).
+ Some parameters inside the source code:
  + description
  + url_mirror
  + url_transformer
  + data dict inside create-* functions