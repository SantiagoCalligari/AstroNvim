<div align="center" id="madewithlua">
    <img src="https://astronvim.github.io/img/logo/astronvim.svg" width="110", height="100">
</div>

<h1 align="center">AstroNvim</h1>

<h4 align="center">
  <a href="https://astronvim.github.io/#%EF%B8%8F-installation">Install</a>
  ·
  <a href="https://astronvim.github.io/#%EF%B8%8F-configuration">Configure</a>
  ·
  <a href="https://astronvim.github.io">Docs</a>
</h4>

<p align="center">
    <a href="https://github.com/AstroNvim/AstroNvim/pulse">
      <img src="https://img.shields.io/github/last-commit/AstroNvim/AstroNvim?style=for-the-badge&logo=github&color=7dc4e4&logoColor=D9E0EE&labelColor=302D41"/>
    </a>
    <a href="https://github.com/AstroNvim/AstroNvim/releases/latest">
      <img src="https://img.shields.io/github/v/release/AstroNvim/AstroNvim?style=for-the-badge&logo=gitbook&color=8bd5ca&logoColor=D9E0EE&labelColor=302D41"/>
	</a>
    <a href="https://github.com/AstroNvim/AstroNvim/stargazers">
      <img src="https://img.shields.io/github/stars/AstroNvim/AstroNvim?style=for-the-badge&logo=apachespark&color=eed49f&logoColor=D9E0EE&labelColor=302D41"/>
    </a>
    <br>
    <a href="https://www.reddit.com/r/AstroNvim/">
      <img src="https://img.shields.io/reddit/subreddit-subscribers/AstroNvim?style=for-the-badge&logo=reddit&color=ee99a0&logoColor=D9E0EE&labelColor=302D41"/>
    </a>
    <a href="https://discord.gg/UcZutyeaFW">
      <img src="https://img.shields.io/discord/939594913560031363?style=for-the-badge&logo=discord&color=cba6f7&logoColor=D9E0EE&labelColor=302D41"/>
    </a>
</p>

<p align="center">
AstroNvim is an aesthetic and feature-rich neovim config that is extensible and easy to use with a great set of plugins
</p>

## 🌟 Preview

![Dashboard Preview Image](https://github.com/AstroNvim/astronvim.github.io/raw/main/static/img/dashboard.png)
![Coding Preview Image](https://github.com/AstroNvim/astronvim.github.io/raw/main/static/img/overview.png)
![Debugging Preview Image](https://github.com/AstroNvim/astronvim.github.io/raw/main/static/img/dap.png)

## ✨ Features

- File explorer with [Neo-tree](https://github.com/nvim-neo-tree/neo-tree.nvim)
- Autocompletion with [Cmp](https://github.com/hrsh7th/nvim-cmp)
- Git integration with [Gitsigns](https://github.com/lewis6991/gitsigns.nvim)
- Statusline with [Heirline](https://github.com/rebelot/heirline.nvim)
- Terminal with [Toggleterm](https://github.com/akinsho/toggleterm.nvim)
- Fuzzy finding with [Telescope](https://github.com/nvim-telescope/telescope.nvim)
- Syntax highlighting with [Treesitter](https://github.com/nvim-treesitter/nvim-treesitter)
- Formatting and linting with [Null-ls](https://github.com/jose-elias-alvarez/null-ls.nvim)
- Language Server Protocol with [Native LSP](https://github.com/neovim/nvim-lspconfig)
- Debug Adapter Protocol with [nvim-dap](https://github.com/mfussenegger/nvim-dap)
- Buffer Line with [bufferline.nvim](https://github.com/akinsho/bufferline.nvim)

## ⚡ Requirements

- [Nerd Fonts](https://www.nerdfonts.com/font-downloads) (_Optional with manual intervention:_ See [Documentation on customizing icons](https://astronvim.github.io/Recipes/icons))
- [Neovim 0.8 (_Not_ including nightly)](https://github.com/neovim/neovim/releases/tag/v0.8.0)
- [Tree-sitter CLI](https://github.com/tree-sitter/tree-sitter/blob/master/cli/README.md) (_Note:_ This is only necessary if you want to use `auto_install` feature with Treesitter)
- A clipboard tool is necessary for the integration with the system clipboard (see [`:help clipboard-tool`](https://neovim.io/doc/user/provider.html#clipboard-tool) for supported solutions)
- Terminal with true color support (for the default theme, otherwise it is dependent on the theme you are using)
- Optional Requirements:
  - [ripgrep](https://github.com/BurntSushi/ripgrep) - live grep telescope search (`<leader>fw`)
  - [lazygit](https://github.com/jesseduffield/lazygit) - git ui toggle terminal (`<leader>tl` or `<leader>gg`)
  - [go DiskUsage()](https://github.com/dundee/gdu) - disk usage toggle terminal (`<leader>tu`)
  - [bottom](https://github.com/ClementTsang/bottom) - process viewer toggle terminal (`<leader>tt`)
  - [Python](https://www.python.org/) - python repl toggle terminal (`<leader>tp`)
  - [Node](https://nodejs.org/en/) - node repl toggle terminal (`<leader>tn`)

> Note when using default theme: For MacOS, the default terminal does not have true color support. You will need to use [iTerm2](https://iterm2.com/) or another [terminal emulator](https://gist.github.com/XVilka/8346728#terminal-emulators) that has true color support.

## 🛠️ Installation

#### Make a backup of your current nvim and shared folder

```shell
mv ~/.config/nvim ~/.config/nvim.bak
mv ~/.local/share/nvim ~/.local/share/nvim.bak
```

#### Clone the repository

```shell
git clone https://github.com/SantiagoCalligari/AstroNvim ~/.config/nvim
nvim +PackerSync
```

## 📦 Basic Setup

#### Install LSP

Enter `:LspInstall` followed by the name of the server you want to install<br>
Example: `:LspInstall pyright`

#### Install language parser

Enter `:TSInstall` followed by the name of the language you want to install<br>
Example: `:TSInstall python`

#### Install Debugger

Enter `:DapInstall` followed by the name of the debugger you want to install<br>
Example: `:DapInstall python`

#### Manage plugins

Run `:PackerClean` to remove any disabled or unused plugins<br>
Run `:PackerSync` to update and clean plugins<br>

#### Update AstroNvim

Run `:AstroUpdate` to get the latest updates from the repository<br>

## 🗒️ Links

[AstroNvim Documentation](https://astronvim.github.io/)
[Core AstroNvim LUA API Documentation](https://astronvim.github.io/AstroNvim/)

- [Basic Usage](https://astronvim.github.io/Basic%20Usage/walkthrough) is given for basic usage
- [Default Mappings](https://astronvim.github.io/Basic%20Usage/mappings) more about the default key bindings
- [Default Plugin Configuration](https://astronvim.github.io/configuration/plugin_defaults) more about the provided plugin defaults
- [Advanced Configuration](https://astronvim.github.io/configuration/config_options) more about advanced configuration

### 📹 Videos

There have been some great review videos released by members of the community! Here are a few:

- [Why I'm quitting VIM by Carlos Mafla](https://www.youtube.com/watch?v=71GDopdc9rw) (Content By: [@gigo6000](https://github.com/gigo6000))
- [Astro Vim - All in one Nvim config!! by John McBride](https://www.youtube.com/watch?v=JQLZ7NJRTEo) (Content By: [@jpmcb](https://github.com/jpmcb))

## ⭐ Credits

Sincere appreciation to the following repositories, plugin authors and the entire neovim community out there that made the development of AstroNvim possible.

- [Plugins](https://astronvim.github.io/acknowledgements#plugins-used-in-astronvim)
- [NvChad](https://github.com/NvChad/NvChad)
- [LunarVim](https://github.com/LunarVim)
- [CosmicVim](https://github.com/CosmicNvim/CosmicNvim)

<div align="center" id="madewithlua">

[![Lua](https://img.shields.io/badge/Made%20with%20Lua-blue.svg?style=for-the-badge&logo=lua)](https://lua.org)

</div>
