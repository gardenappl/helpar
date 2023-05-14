Helps you extract archives and list their contents.


## TODO: readme

It's supposed to be a helpful and also educational tool. Suggests the simplest command for the appropriate archive format, while also being non-destructive by default (does not overwrite existing files, does not delete the archive after extraction, etc).

![Screenshot](screenshot.png)

Supported archive and compression formats:

|                      File extenstion                     | Tools |
|                      --------------:                     | :--- |
| `.tar`, `.tar.*`, `.tgz`, `.tbz`, `.txz`, `.tlz`, `.tzo` | `tar`, `bsdtar`, `7z` |
| `.zip`                                                   | `unzip` (`zipinfo`), `bsdtar`, `7z` |
| `.rar`                                                   | `unrar`, `bsdtar`, `7z` |
| `.7z`                                                    | `7z`, `bsdtar` |
| `.arj`                                                   | `unarj`², `7z` |
| `.bz2`³, `.bz`³                                          | `bzip2` (`bunzip2`, `bzcat`), `7z`
| `.cpio`                                                  | `cpio`, `bsdtar`, `7z` |
| `.deb`                                                   | `dpkg-deb`¹ |
| `.gz`                                                    | `gzip` (`gunzip2`, `zcat`), `7z` |
| `.lha`                                                   | `lha`¹, `lhasa`¹, `bsdtar`, `7z` |
| `.lrz`³                                                  | `lrzip` (`lrunzip`, `lrzcat`) |
| `.lz`³                                                   | `lzip`, `7z` |
| `.lz4`³                                                  | `lz4` (`unlz4`), `7z` |
| `.lzma`³                                                 | `xz` (`unlzma`, `lzcat`), `7z` |
| `.lzo`                                                   | `lzop`¹ |
| `.xz`³                                                   | `xz` (`unxz`, `xzcat`), `7z` |
| `.zst`³                                                  | `zstd` (`unzstd`), `7z` |
| `.exe` (PE)                                              | `7z` |
| `.Z`³                                                    | `uncompress`, `7z` |
| `.pax`                                                   | TODO |
| [`.hrx`](https://github.com/google/hrx)                  | TODO |
| Others (fallback)                                        | `bsdtar`, `7z` |

Notes:
1. Tool with limited support.
2. Tool with very limited support.
3. Single-file compression format. Sometimes these compression formats can store a filename, sometimes they don't (in which case the `list` command is useless).

