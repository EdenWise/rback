### Description

**rback** is a generic backup and restore script.  It wraps common functions of **rsync** to aggragate backup necessities.  **rback** defines:

1. The copy options.
2. The *source* and *destination* directories.
3. The *file*, *folders*... to *include* or *exclude*.

**rback** is repository-based to allow for multiple backup types (like full system backups, configurations...), and is only for local backups (i.e. the same computer that it resides on).  Additionaly, **rback** includes a *diff* method for working with text files.

### Usage

```sh
rback - a generic, local, rsync-based, backup and restore script
  -r, --repo    - repository select                     : -R repository new
  -i, --include - include list add files, folders...    : -I include list edit
  -e, --exclude - exclude list add files, folders...    : -E exclude list edit
  -x, --xecute  - execute a: restore, backup, or diff
  = overrides  =
  -c, --confdir - configuration dir. from livecd, e.g.  : -C configuration edit
  -s, --srcdir  - source directory,  alternate specify
  -d, --dstdir  - destination dir.,  alternate specify
  -j, --justdo  - no confirm
```

For more information, rtfw (read the fun manual).
