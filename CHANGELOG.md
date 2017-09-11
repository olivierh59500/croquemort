# Changelog

## 2.0.0 (TBD)

Mandatory migrations from `1.0.0` to `2.0.0`:

```bash
# Launch the migrations service - logs will be displayed here
nameko run croquemort.migrations --config config.yaml
# In another terminal session
nameko shell
>>> n.rpc.migrations.migrate_from_1_to_2()
```

### Breaking changes

- Hash prefixes in Redis DB
  [#26](https://github.com/opendatateam/croquemort/issues/26)
  — associated migration: `add_hash_prefixes`
- Redirection support
  [#1](https://github.com/opendatateam/croquemort/issues/1)
  — associated migration: `migrate_urls_redirect`

### Features

- Webhook support
  [#24](https://github.com/opendatateam/croquemort/issues/24)

### Misc

- Remove logbook in favor of logging
  [#29](https://github.com/opendatateam/croquemort/issues/29)

## 1.0.0 (2017-01-23)

- Initial version