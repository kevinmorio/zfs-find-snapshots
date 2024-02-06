# zfs-find-snapshots

**Find all ZFS snapshots containing a file or directory.**

``` shell
$ zfs-find-snapshots fileA
tank@2024-01-01
tank@2024-01-02
tank@2024-01-03
```

## Usage

### List all snapshots containing a file or directory

``` shell
$ zfs-find-snapshots <file|directory>
```

### Delete all snapshots containing a file or directory

``` shell
$ zfs-find-snapshots <file|directory> | xargs -I {} zfs destroy
```

> :warning: **Note**: This operation may cause data loss! Ensure you know what you're doing.

###
