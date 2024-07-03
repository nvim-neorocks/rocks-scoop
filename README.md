# :ice_cream: rocks-scoop :ice_cream:

[`scoop.sh`](https://scoop.sh/) buckets for use with rocks.nvim.

> [!WARNING]
>
> This is used in our [rocks-binaries](https://github.com/nvim-neorocks/rocks-binaries)
> GitHub Actions CI for Windows.
>
> We don't know how well it will work on your machine.

## :bucket: Included buckets

- lua 5.1 + C libraries
- luarocks

## :pencil: Requirements

- [Scoop](https://scoop.sh/)
- A [Microsoft C/C++ compiler](https://learn.microsoft.com/en-us/cpp/build/building-on-the-command-line?view=msvc-170)

## :inbox_tray: Installation

```sh
scoop bucket add neorocks-scoop https://github.com/nvim-neorocks/rocks-scoop.git
scoop install neorocks-scoop/luarocks
```
