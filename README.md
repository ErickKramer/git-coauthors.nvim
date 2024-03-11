# Git-coauthors.nvim

This is a telescope extension for adding co-authors in your git commits. This
works by looking at anyone that has committed to your repo. You can fuzzy find
and multiselect the results.

## 🧰 Installation

[lazy.nvim](https://github.com/folke/lazy.nvim)

```lua
{
	"ErickKramer/git-coauthors.nvim",
	dependencies = {
		"nvim-telescope/telescope.nvim",
	},
},
```

- Register the extension with telescope

```lua
require('telescope').load_extension('coauthors')
```

- Add keymaps

```lua
vim.keymap.set("n", "<leader>ga", ":Telescope coauthors<CR>", { desc = "[G]it co-[A]uthors" })
```

## Usage

The selected authors are inserted in the current bufffer.

For multi-selection press `Tab` at each author you want to add

## Disclaimer

This a slightly modified version from the [original plugin](https://github.com/cwebster2/github-coauthors.nvim)
