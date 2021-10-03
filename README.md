Helps you extract archives and list their contents.


## TODO: readme

It's supposed to be a helpful and also educational tool. Suggests the simplest command for the appropriate archive format, while also being non-destructive by default (does not overwrite existing files, does not delete the archive after extraction, etc).

![Screenshot](screenshot.png)

Supported archive and compression formats:

| File extenstion | Tool |
| --------------- | :--- |
| `.zip` | `unzip` |
| `.rar` | `unrar` |
| `.7z` | `7z` |
| `.tar`, `.tar.gz`, `.tgz`, `.tbz`, `.txz`, `.tlz`, `.tzo`, `.tar.*` | `tar` |
| `.bz2`, `.bz` | `bzip2` |
| `.gz` | `gzip` |
| `.xz`, `.lzma` | `xz` |
| `.lz` | `lzip` |
| `.lzo` | `lzop` |
| `.Z` | `uncompress` |
| Everything else | `7z` |

