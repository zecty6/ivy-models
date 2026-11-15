# Ivy models

Model files that the Ivy video editor downloads on demand. They are attached to the
releases of this repository; there is no source code here.

Ivy checks every file it downloads against a SHA-256 checksum built into the application
and keeps it only if it matches.

## Release `models-1`

### `colour_eccv16` — colour for black-and-white footage

| File | Bytes | SHA-256 |
| --- | --- | --- |
| `colour_eccv16.ncnn.bin` | 64518824 | `5b321a85f559bacf501df489ec4ee97a5c3ec57db512ff8a1012784c86ba1c8e` |
| `colour_eccv16.ncnn.param` | 3769 | `74716935b3407b9ba1c59f443ee245ca26aa95a7f27a4cc903df5c6190ff8e05` |

The network of Richard Zhang, Phillip Isola and Alexei A. Efros, "Colorful Image
Colorization" (ECCV 2016), https://github.com/richzhang/colorization, BSD-2-Clause
(see `LICENSE-colour_eccv16.txt`).

The files are the authors' official checkpoint
`colorization_release_v2-9b330a0b.pth`
(SHA-256 `9b330a0bae53f4ded77b1e23defbf78beaa09c10ebc4c4999e8e4f4a160b93f9`)
converted to the ncnn format with pnnx, with 16-bit weights. The weights are otherwise
unchanged.
