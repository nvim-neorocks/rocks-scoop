# Scoop Bucket

[`scoop.sh`](https://scoop.sh/) buckets for use with rocks.nvim.

> [!WARNING]
>
> This is used in our [rocks-binaries](https://github.com/nvim-neorocks/rocks-binaries)
> GitHub Actions CI for Windows.
>
> We don't know how well it will work on your machine.

## Buckets

- lua 5.1 + C libraries
- luarocks

## Usage

```sh
scoop bucket add neorocks-scoop https://github.com/nvim-neorocks/rocks-scoop.git
scoop install neorocks-scoop/luarocks
```
