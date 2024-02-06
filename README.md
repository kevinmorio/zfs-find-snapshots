# zfs-find-snapshots

**Find all ZFS snapshots containing a file or directory.**

## Usage

### List all snapshots containing a file or directory

``` shell
zfs-find-snapshots <file|directory>
```

### Delete all snapshots containing a file or directory

``` shell
zfs-find-snapshots <file|directory> | xargs -I {} zfs destroy
```

> :warning: **Note**: This operation may cause data loss! Ensure you know what you're doing.

###
