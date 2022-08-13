Helps you extract archives and list their contents.


## TODO: readme

It's supposed to be a helpful and also educational tool. Suggests the simplest command for the appropriate archive format, while also being non-destructive by default (does not overwrite existing files, does not delete the archive after extraction, etc).

![Screenshot](screenshot.png)

Supported archive and compression formats:

| File extenstion | Tool | Notes |
| --------------: | :--- | ------------------ |
| `.tar`, `.tar.*`, `.tgz`, `.tbz`, `.txz`, `.tlz`, `.tzo` | `tar` |
| `.zip` | `unzip` |
| `.rar` | `unrar` |
| `.7z` | `7z` |
| `.arj` | `unarj` | Very limited support |
| `.bz2`, `.bz` | `bzip2` (`bunzip2`, `bzcat`) | Single-file |
| `.cpio` | `cpio` |
| `.deb` | `dpkg-deb` | Limited support |
| `.gz` | `gzip` (`gunzip2`, `zcat`) | Single-file |
| `.lha` | `lha` or `lhasa` | Limited support |
| `.lrz` | `lrzip` (`lrunzip`, `lrzcat`) | Single-file |
| `.lz` | `lzip` | Single-file |
| `.lz4` | `lz4` (`unlz4`) | Single-file |
| `.lzma` | `xz` (`unlzma`, `lzcat`) | Single-file |
| `.lzo` | `lzop` | Limited support |
| `.xz` | `xz` (`unxz`, `xzcat`) | Single-file |
| `.zst` | `zstd` (`unzstd`) | Single-file |
| `.Z` | `uncompress` | Single-file |
| Everything else | `7z` | N/A |

* "Single-file" refers to compression tools which don't support archival (only work on single files). The `list` command is useless in these cases.

