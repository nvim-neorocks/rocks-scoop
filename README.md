# :ice_cream: rocks-scoop :ice_cream:

[`scoop.sh`](https://scoop.sh/) buckets for use with [rocks.nvim](https://github.com/nvim-neorocks/rocks.nvim) and [lazy.nvim](https://github.com/folke/lazy.nvim) on Windows.

> [!WARNING]
>
> This is used in our [rocks-binaries](https://github.com/nvim-neorocks/rocks-binaries)
> GitHub Actions CI for Windows.
>
> We don't know how well it will work on your machine.

## :construction: The problem

LuaRocks support for Neovim is an absolute headache on Windows.
This has the following reasons:

- Neovim uses luajit, which has the Lua 5.1 API.
- Most luarocks packages are bundled with Lua 5.4, which is incompatible.
- Even if you install luajit or Lua 5.1 and configure luarocks to use it,
  you will [likely run into issues](https://github.com/luarocks/luarocks/issues/1656),
  because the luarocks Windows all-in-one executable
  has been compiled against Lua 5.4.

## :rocket: The solution

Compile luarocks against Lua 5.1.

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
