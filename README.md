# Ansible Role: Backup Directory

BAcks up a given directory daily.  Keeps the last 30 days of backups by default.

## Requirements

None

## Role Variables

### Main Variables

| Name | Details |
| --- | --- |
| `parent_directory` | The full parent directory of the actual directory you want to backup.  For example, if you want to backup `/usr/bin/local`, this should be set to '/usr/bin' |
| `directory` | The directory within the parent (given above) that should be backed up.  Using the same example as above, this would be `local` |

### Default Variables

| Name | Default Value | Details |
| --- | --- | --- |
| `retention_days` | `30` | Number of days to keep backups |

## License

MIT
