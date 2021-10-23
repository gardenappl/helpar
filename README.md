Helps you extract archives and list their contents.


## TODO: readme

It's supposed to be a helpful and also educational tool. Suggests the simplest command for the appropriate archive format, while also being non-destructive by default (does not overwrite existing files, does not delete the archive after extraction, etc).

![Screenshot](screenshot.png)

Supported archive and compression formats:

| File extenstion | Tool | Compression only\* |
| --------------- | :--- | :--------------- |
| `.tar`, `.tar.*`, `.tgz`, `.tbz`, `.txz`, `.tlz`, `.tzo` | `tar` |
| `.zip` | `unzip` |
| `.rar` | `unrar` |
| `.7z` | `7z` |
| `.bz2`, `.bz` | `bzip2` (`bunzip2`, `bzcat`) | Yes |
| `.cpio` | `.cpio` |
| `.gz` | `gzip` (`gunzip2`, `zcat`) | Yes |
| `.lrz` | `lrzip` (`lrunzip`, `lrzcat`) | Yes |
| `.lz` | `lzip` | Yes |
| `.lz4` | `lz4` (`unlz4`) | Yes |
| `.lzma` | `xz` (`unlzma`, `lzcat`) | Yes |
| `.lzo` | `lzop` |
| `.xz` | `xz` (`unxz`, `xzcat`) | Yes |
| `.zst` | `zstd` (`unzstd`) | Yes |
| `.Z` | `uncompress` | Yes |
| Everything else | `7z` | N/A |

* "Compression-only" refers to compression tools which don't support archival (only work on single files). The `help-lsarchive` command is useless in these cases.

