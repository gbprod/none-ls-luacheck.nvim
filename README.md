# none-ls-luacheck.nvim

[Luacheck](https://github.com/mpeterv/luacheck) diagnostics source for [none-ls.nvim](https://github.com/nvimtools/none-ls.nvim).

Since this diagnostic was deprecated from [none-ls.nvim](https://github.com/nvimtools/none-ls.nvim)
(see [this issue](https://github.com/nvimtools/none-ls.nvim/issues/58)) because [selene](https://github.com/Kampfkarren/selene) is a better alternative,
this repository allows to keep using [Luacheck](https://github.com/mpeterv/luacheck) with [none-ls.nvim](https://github.com/nvimtools/none-ls.nvim).

**Note:** This plugin is not intended to be used alone, it is a dependency of none-ls.nvim.

## 📦 Installation

This should be used as a dependency of **none-ls.nvim**.

### [lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{
  {
    "nvimtools/none-ls.nvim",
    config = function()
        require("null-ls").register(require("none-ls-luacheck.diagnostics.luacheck"))
    end,
    dependencies = {
        "gbprod/none-ls-luacheck.nvim",
    },
  },
}
```
