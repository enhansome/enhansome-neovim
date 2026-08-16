# Awesome Neovim with stars

<a href="https://neovim.io/"><img src="https://neovim.io/logos/neovim-mark-flat.png" align="right" width="144"/></a>

> A collection of awesome Neovim plugins. Mostly targeting Neovim specific features.
> This means Vim-compatible plugins are not listed here.

[Neovim](https://neovim.io/) is a Vim-based text editor engineered for extensibility and usability, to encourage new applications and contributions.
It has some [builtin plugins](https://neovim.io/doc/user/plugins.html#plugins) as well as a rich API for many more to be developed.

## Contents

* [Plugin Manager](#plugin-manager)
* [LSP](#lsp)
  * [Diagnostics](#diagnostics)
* [Completion](#completion)
* [AI](#ai)
* [Programming Languages Support](#programming-languages-support)
  * [Golang](#golang)
  * [Web Development](#web-development)
  * [Markdown and LaTeX](#markdown-and-latex)
* [Language](#language)
* [Syntax](#syntax)
* [Snippet](#snippet)
* [Register](#register)
* [Marks](#marks)
* [Search](#search)
* [Fuzzy Finder](#fuzzy-finder)
* [File Explorer](#file-explorer)
* [Project](#project)
* [Buffers](#buffers)
* [Color](#color)
* [Colorscheme](#colorscheme)
  * [Colorscheme Creation](#colorscheme-creation)
  * [Colorscheme Switchers](#colorscheme-switchers)
* [Bars and Lines](#bars-and-lines)
  * [Statusline](#statusline)
  * [Tabline](#tabline)
  * [Cursorline](#cursorline)
* [Startup](#startup)
* [Icon](#icon)
* [Media](#media)
* [Note Taking](#note-taking)
* [Utility](#utility)
  * [CSV Files](#csv-files)
* [Animation](#animation)
* [Terminal Integration](#terminal-integration)
* [Debugging](#debugging)
  * [Quickfix](#quickfix)
* [Test](#test)
* [Code Runner](#code-runner)
* [Neovim Lua Development](#neovim-lua-development)
* [Fennel](#fennel)
* [Dependency Management](#dependency-management)
* [Git](#git)
  * [GitHub](#github)
* [Motion](#motion)
  * [Tree-sitter Based](#tree-sitter-based)
* [Keybinding](#keybinding)
* [Scrolling](#scrolling)
  * [Scrollbar](#scrollbar)
* [Editing Support](#editing-support)
  * [Comment](#comment)
  * [Folding](#folding)
* [Formatting](#formatting)
  * [Indent](#indent)
* [Command Line](#command-line)
* [Session](#session)
* [Remote Development](#remote-development)
* [Live Preview](#live-preview)
* [Split and Window](#split-and-window)
  * [Tmux](#tmux)
* [Game](#game)
  * [Competitive Programming](#competitive-programming)
* [Toys](#toys)
* [Workflow](#workflow)
  * [Stats Tracking](#stats-tracking)
* [Database](#database)
* [Pre-made Configuration](#pre-made-configuration)
* [External](#external)
  * [Version Manager](#version-manager)
  * [Plugin Template](#plugin-template)
  * [OS-specific](#os-specific)
* [Wishlist](#wishlist)
* [UI](#ui)
* [External Resource](#external-resource)

## Plugin Manager

* [folke/lazy.nvim](https://github.com/folke/lazy.nvim) ⭐ 21,413 | 🐛 67 | 🌐 Lua | 📅 2026-06-29 - A modern plugin manager, featuring a graphical interface, async execution, a lockfile and more.
  * [cosmicbuffalo/super\_lazy.nvim](https://github.com/cosmicbuffalo/super_lazy.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - An extension to `folke`'s `lazy.nvim`, enables use of multiple lockfiles for large teams that want to combine your shared/personal configurations.
* [nvim-mini/mini.nvim#mini.deps](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-deps.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for managing other plugins. Uses Git and built-in packages to install, update, clean, and snapshot plugins.
* [lumen-oss/rocks.nvim](https://github.com/lumen-oss/rocks.nvim) ⭐ 1,059 | 🐛 56 | 🌐 Lua | 📅 2026-08-13 - A modern approach to plugin management using LuaRocks, inspired by Cargo.
* [savq/paq-nvim](https://github.com/savq/paq-nvim) ⭐ 709 | 🐛 7 | 🌐 Lua | 📅 2025-03-30 - Package manager written in Lua.
* [alex-popov-tech/store.nvim](https://github.com/alex-popov-tech/store.nvim) ⭐ 369 | 🐛 0 | 🌐 Lua | 📅 2026-07-22 - Plugins discovery tool with hourly updated database, and one-key installation for `lazy.nvim` and `vim.pack`.
* [lewis6991/pckr.nvim](https://github.com/lewis6991/pckr.nvim) ⭐ 347 | 🐛 8 | 🌐 Lua | 📅 2025-09-25 - Spiritual successor of `wbthomason/packer.nvim`.
* [zuqini/zpack.nvim](https://github.com/zuqini/zpack.nvim) ⭐ 146 | 🐛 0 | 🌐 Lua | 📅 2026-08-05 - A thin layer on top of `vim.pack` to support lazy-loading and `lazy.nvim`'s declarative spec.
* [wsdjeg/nvim-plug](https://github.com/wsdjeg/nvim-plug) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2026-07-18 - Asynchronous plugin manager written in Lua.
* [piersolenski/plugin-addict.nvim](https://github.com/piersolenski/plugin-addict.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - A stupidly simple way to quickly install plugins.
* [alyxshang/nuwa.nvim](https://source.alyxshang.boo/alyxshang/nuwa.nvim) - A light package manager.
* [OriginCoderPulse/synapse.nvim](https://github.com/OriginCoderPulse/synapse.nvim) - A modern, lightweight plugin manager with beautiful UI, intelligent dependency management, tag/branch support, and post-install command execution.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## LSP

**(requires Neovim 0.5)**

* [Dan7h3x/signup.nvim](https://github.com/Dan7h3x/signup.nvim) ⭐ 65 | 🐛 0 | 🌐 Lua | 📅 2026-01-27 - a little smart `lsp_signature` helper with awesome features.
* [romus204/referencer.nvim](https://github.com/romus204/referencer.nvim) ⭐ 49 | 🐛 2 | 🌐 Lua | 📅 2025-11-19 - Lightweight, asynchronous that uses the LSP to show references to functions, methods, types and other.
* [nvim-pio](https://github.com/batoaqaa/nvim-pio) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-08-11 - Asynchronous, zero-hardcoding bridge between PlatformIO and the `clangd` LSP.

<!--lint disable awesome-spell-check-->

* [neovim/nvim-lspconfig](https://github.com/neovim/nvim-lspconfig) ⭐ 13,878 | 🐛 36 | 🌐 Lua | 📅 2026-08-13 - Quickstart configurations for the LSP client.

<!--lint enable awesome-spell-check-->

* [nvimdev/lspsaga.nvim](https://github.com/nvimdev/lspsaga.nvim) ⭐ 3,797 | 🐛 98 | 🌐 Lua | 📅 2026-07-16 - A light-weight LSP plugin based on the built-in LSP with a highly performant UI.
* [mfussenegger/nvim-lint](https://github.com/mfussenegger/nvim-lint) ⭐ 2,774 | 🐛 45 | 🌐 Lua | 📅 2026-08-13 - An asynchronous linter plugin, complementary to the built-in Language Server Protocol support.
* [j-hui/fidget.nvim](https://github.com/j-hui/fidget.nvim) ⭐ 2,588 | 🐛 17 | 🌐 Lua | 📅 2026-06-21 - Standalone UI for LSP progress.
* [ray-x/lsp\_signature.nvim](https://github.com/ray-x/lsp_signature.nvim) ⭐ 2,371 | 🐛 88 | 🌐 Lua | 📅 2026-05-19 - LSP signature hint when you type.
* [stevearc/aerial.nvim](https://github.com/stevearc/aerial.nvim) ⭐ 2,336 | 🐛 73 | 🌐 Lua | 📅 2026-06-02 - A code outline window for skimming and quick navigation.
* [onsails/lspkind.nvim](https://github.com/onsails/lspkind.nvim) ⭐ 1,691 | 🐛 15 | 🌐 Lua | 📅 2026-01-29 - The plugin adds VSCode-like icons to LSP completions.
* [ray-x/navigator.lua](https://github.com/ray-x/navigator.lua) ⭐ 1,401 | 🐛 23 | 🌐 Lua | 📅 2026-08-13 - Learn existing code quickly and navigate code like a breeze. A swiss army knife makes exploring LSP and Tree-sitter symbols a piece of cake.
* [rmagatti/goto-preview](https://github.com/rmagatti/goto-preview) ⭐ 1,054 | 🐛 11 | 🌐 Lua | 📅 2025-12-26 - Previewing native LSP's goto definition calls in floating windows.
* [hedyhli/outline.nvim](https://github.com/hedyhli/outline.nvim) ⭐ 1,042 | 🐛 35 | 🌐 Lua | 📅 2026-05-29 - A significantly enhanced and refactored fork of `symbols-outline.nvim`.
* [b0o/SchemaStore.nvim](https://github.com/b0o/SchemaStore.nvim) ⭐ 1,022 | 🐛 11 | 🌐 Lua | 📅 2026-08-14 - Provide access to the [SchemaStore](https://github.com/SchemaStore/schemastore) ⭐ 3,819 | 🐛 201 | 🌐 JavaScript | 📅 2026-08-14 catalog.
* [kosayoda/nvim-lightbulb](https://github.com/kosayoda/nvim-lightbulb) ⭐ 892 | 🐛 6 | 🌐 Lua | 📅 2026-04-27 - The plugin shows a lightbulb in the sign column whenever a `textDocument/codeAction` is available at the current cursor position.
* [smjonas/inc-rename.nvim](https://github.com/smjonas/inc-rename.nvim) ⭐ 863 | 🐛 10 | 🌐 Lua | 📅 2026-07-30 - Provides an incremental LSP rename command based on the command-preview feature.
* [aznhe21/actions-preview.nvim](https://github.com/aznhe21/actions-preview.nvim) ⭐ 517 | 🐛 10 | 🌐 Lua | 📅 2026-04-22 - Fully customizable previewer for LSP code actions.
* [jubnzv/virtual-types.nvim](https://github.com/jubnzv/virtual-types.nvim) ⭐ 421 | 🐛 2 | 🌐 Lua | 📅 2023-04-07 - Show type annotations as virtual text.
* [ojroques/nvim-lspfuzzy](https://github.com/ojroques/nvim-lspfuzzy) ⭐ 355 | 🐛 0 | 🌐 Lua | 📅 2026-05-01 - A small plugin to make the LSP client use FZF.
* [tamago324/nlsp-settings.nvim](https://github.com/tamago324/nlsp-settings.nvim) ⭐ 336 | 🐛 10 | 🌐 Lua | 📅 2026-07-29 - Setup LSP with JSON or YAML files.
* [gfanto/fzf-lsp.nvim](https://github.com/gfanto/fzf-lsp.nvim) ⭐ 241 | 🐛 15 | 🌐 Lua | 📅 2024-08-07 - Enable the power of FZF fuzzy search for the built-in LSP.
* [marilari88/twoslash-queries.nvim](https://github.com/marilari88/twoslash-queries.nvim) ⭐ 175 | 🐛 3 | 🌐 Lua | 📅 2025-09-26 - Provide inline virtual text displaying TypeScript types for the inspected variables.
* [hasansujon786/nvim-navbuddy](https://github.com/hasansujon786/nvim-navbuddy) ⭐ 83 | 🐛 1 | 🌐 Lua | 📅 2025-05-11 - A simple popup display that provides breadcrumbs like navigation feature but in keyboard centric manner, inspired by the `ranger` file manager.
* [retran/meow.yarn.nvim](https://github.com/retran/meow.yarn.nvim) ⭐ 79 | 🐛 3 | 🌐 Lua | 📅 2026-04-19 - Interactive LSP type and call hierarchy explorer with a tree view, live preview, navigation breadcrumbs, and a custom node renderer.
* [jakewvincent/texmagic.nvim](https://github.com/jakewvincent/texmagic.nvim) ⭐ 59 | 🐛 4 | 🌐 Lua | 📅 2026-03-02 - Enhance the lspconfig settings for Texlab by defining any number of custom LaTeX build engines and selecting them with magic comments.

<!--lint disable double-link-->

* [scalameta/nvim-metals](https://github.com/scalameta/nvim-metals) ⭐ 566 | 🐛 22 | 🌐 Lua | 📅 2026-07-02 - Provides a better experience while using [Metals](https://scalameta.org/metals/), the Scala Language Server, using the built-in LSP support.

<!--lint enable double-link-->

* [mason-org/mason.nvim](https://github.com/mason-org/mason.nvim) ⭐ 10,435 | 🐛 275 | 🌐 Lua | 📅 2026-06-19 - Easily install and manage LSP servers, DAP servers, linters, and formatters.
* [nvimtools/none-ls.nvim](https://github.com/nvimtools/none-ls.nvim) ⭐ 3,257 | 🐛 12 | 🌐 Lua | 📅 2026-08-10 - A reloaded `null-ls.nvim` to use your editor as a language server to inject LSP diagnostics, code actions, and more via Lua.
* [mrcjkb/rustaceanvim](https://github.com/mrcjkb/rustaceanvim) ⭐ 3,078 | 🐛 20 | 🌐 Lua | 📅 2026-08-16 - A heavily modified fork of rust-tools.nvim that does not require a `setup` call and does not depend on nvim-lspconfig.
* [rachartier/tiny-inline-diagnostic.nvim](https://github.com/rachartier/tiny-inline-diagnostic.nvim) ⭐ 1,719 | 🐛 0 | 🌐 Lua | 📅 2026-07-05 - Display prettier diagnostic messages. Display one line diagnostic messages where the cursor is, with icons and colors.
* [mfussenegger/nvim-jdtls](https://github.com/mfussenegger/nvim-jdtls) ⭐ 1,492 | 🐛 3 | 🌐 Lua | 📅 2026-05-20 - Extensions for the built-in LSP support for the Eclipse JDT Language Server.
* [DNLHC/glance.nvim](https://github.com/DNLHC/glance.nvim) ⭐ 924 | 🐛 22 | 🌐 Lua | 📅 2025-06-16 - A pretty window for previewing, navigating and editing your LSP locations.
* [jmbuhr/otter.nvim](https://github.com/jmbuhr/otter.nvim) ⭐ 893 | 🐛 19 | 🌐 Lua | 📅 2026-07-08 - Provides LSP features and a nvim-cmp completion source for languages embedded in other documents.
* [mrcjkb/haskell-tools.nvim](https://github.com/mrcjkb/haskell-tools.nvim) ⭐ 604 | 🐛 21 | 🌐 Lua | 📅 2026-08-15 - Seamless integration for Haskell development tools like `haskell-language-server` and Hoogle.
* [zeioth/garbage-day.nvim](https://github.com/Zeioth/garbage-day.nvim) ⭐ 525 | 🐛 4 | 🌐 Lua | 📅 2026-02-25 - Garbage collector that stops inactive LSP clients to free RAM.
* [Wansmer/symbol-usage.nvim](https://github.com/Wansmer/symbol-usage.nvim) ⭐ 500 | 🐛 2 | 🌐 Lua | 📅 2026-04-06 - Display references, definitions and implementations of document symbols.
* [rachartier/tiny-code-action.nvim](https://github.com/rachartier/tiny-code-action.nvim) ⭐ 493 | 🐛 0 | 🌐 Lua | 📅 2026-04-25 - Provides a simple way to run and visualize code actions with Telescope.
* [soulis-1256/eagle.nvim](https://github.com/soulis-1256/eagle.nvim) ⭐ 358 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - Mouse-hover LSP hints.
* [VidocqH/lsp-lens.nvim](https://github.com/VidocqH/lsp-lens.nvim) ⭐ 324 | 🐛 21 | 🌐 Lua | 📅 2024-08-09 - Display function references above function definition like IDEA codelens.
* [creativenull/efmls-configs-nvim](https://github.com/creativenull/efmls-configs-nvim) ⭐ 319 | 🐛 1 | 🌐 Lua | 📅 2026-08-11 - An unofficial collection of linters and formatters configured for efm-langserver to work with built-in LSP.
* [jinzhongjia/LspUI.nvim](https://github.com/jinzhongjia/LspUI.nvim) ⭐ 292 | 🐛 0 | 🌐 Lua | 📅 2026-04-28 - A modern and useful UI that wraps LSP operations.
* [Fildo7525/pretty\_hover](https://github.com/Fildo7525/pretty_hover) ⭐ 250 | 🐛 2 | 🌐 Lua | 📅 2026-05-22 - Highly customizable hover formatter, extendable to blink.cmp. As native hover supports multiple LSP servers.
* [chrisgrieser/nvim-lsp-endhints](https://github.com/chrisgrieser/nvim-lsp-endhints) ⭐ 247 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Display LSP inlay hints at the end of the line, rather than within the line.
* [linrongbin16/lsp-progress.nvim](https://github.com/linrongbin16/lsp-progress.nvim) ⭐ 238 | 🐛 1 | 🌐 Lua | 📅 2026-02-02 - A performant LSP progress status.
* [junnplus/lsp-setup.nvim](https://github.com/junnplus/lsp-setup.nvim) ⭐ 235 | 🐛 2 | 🌐 Lua | 📅 2025-05-15 - A simple wrapper for `nvim-lspconfig` and `mason-lspconfig` to easily setup LSP servers.
* [hinell/lsp-timeout.nvim](https://github.com/hinell/lsp-timeout.nvim) ⭐ 233 | 🐛 0 | 🌐 Lua | 📅 2025-04-04 - Automatically start/stop idle/unused LSP servers; keeps RAM usage low.
* [amrbashir/nvim-docs-view](https://github.com/amrbashir/nvim-docs-view) ⭐ 188 | 🐛 1 | 🌐 Lua | 📅 2026-06-11 - Display LSP hover documentation in a side panel.
* [barreiroleo/ltex\_extra.nvim](https://github.com/barreiroleo/ltex_extra.nvim) ⭐ 188 | 🐛 11 | 🌐 Lua | 📅 2025-11-01 - LTeX LSP extension providing external file handling (rules and dictionaries).
* [alexpasmantier/pymple.nvim](https://github.com/alexpasmantier/pymple.nvim) ⭐ 153 | 🐛 4 | 🌐 Lua | 📅 2025-12-20 - Refactor Python imports on file move/rename.
* [vxpm/ferris.nvim](https://github.com/vxpm/ferris.nvim) ⭐ 123 | 🐛 1 | 🌐 Lua | 📅 2025-08-04 - Interact with Rust-Analyzer's LSP extensions.
* [error311/wayfinder.nvim](https://github.com/error311/wayfinder.nvim) ⭐ 120 | 🐛 1 | 🌐 Lua | 📅 2026-08-08 - Guided code exploration from the current symbol with a keepable trail.
* [creativenull/diagnosticls-configs-nvim](https://github.com/creativenull/diagnosticls-configs-nvim) ⭐ 94 | 🐛 2 | 🌐 Lua | 📅 2025-11-12 - An unofficial collection of linters and formatters configured for diagnostic-languageserver to work with built-in LSP.
* [esmuellert/nvim-eslint](https://github.com/esmuellert/nvim-eslint) ⭐ 92 | 🐛 8 | 🌐 Python | 📅 2026-02-21 - Bundle VSCode ESLint language server and utilize the native LSP client to provide a all-in-one ESLint experience.
* [lopi-py/luau-lsp.nvim](https://github.com/lopi-py/luau-lsp.nvim) ⭐ 90 | 🐛 0 | 🌐 Lua | 📅 2026-02-25 - A luau-lsp extension to improve your experience.
* [yarospace/dev-tools.nvim](https://github.com/yarospace/dev-tools.nvim) ⭐ 87 | 🐛 0 | 🌐 Lua | 📅 2025-11-01 - In-process LSP server for custom code actions, enhanced actions picker, community actions library and a convenient interface to create your own actions.
* [stevanmilic/nvim-lspimport](https://github.com/stevanmilic/nvim-lspimport) ⭐ 82 | 🐛 7 | 🌐 Lua | 📅 2024-07-20 - Automatically resolves imports for undefined terms. Useful with `pyright` language server.
* [ranjithshegde/ccls.nvim](https://github.com/ranjithshegde/ccls.nvim) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2026-04-10 - Use off-spec extensions of ccls LSP and browse AST.
* [Kasama/nvim-custom-diagnostic-highlight](https://github.com/Kasama/nvim-custom-diagnostic-highlight) ⭐ 62 | 🐛 0 | 🌐 Lua | 📅 2023-05-09 - Inline diagnostics popup-highlight much like `coc-nvim` but based on `vim.diagnostic`.
* [mawkler/refjump.nvim](https://github.com/mawkler/refjump.nvim) ⭐ 61 | 🐛 2 | 🌐 Lua | 📅 2025-12-23 - Jump to next/previous LSP reference for item under cursor with `]r`/`[r`.
* [nemanjamalesija/ts-expand-hover.nvim](https://github.com/nemanjamalesija/ts-expand-hover.nvim) ⭐ 61 | 🐛 2 | 🌐 Lua | 📅 2026-03-06 - Progressively expand and collapse TypeScript type aliases inside the hover float.
* [chojs23/ts-bridge](https://github.com/chojs23/ts-bridge) ⭐ 41 | 🐛 0 | 🌐 Rust | 📅 2026-01-06 - TypeScript language server shim that bridges the built-in LSP client with `tsserver`.
* [LukasPietzschmann/boo.nvim](https://github.com/LukasPietzschmann/boo.nvim) ⭐ 39 | 🐛 4 | 🌐 Lua | 📅 2024-06-27 - Quickly pop-up some LSP-powered information of the thing your cursor is on.
* [Zeioth/none-ls-autoload.nvim](https://github.com/Zeioth/none-ls-autoload.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2025-06-24 - Auto-load/unload `none-ls` sources installed with `mason`, with support for built-in and external sources.
* [Crysthamus/nvim-file-operations](https://github.com/Crysthamus/nvim-file-operations) ⭐ 19 | 🐛 1 | 🌐 Lua | 📅 2026-07-05 - Add support for workspace file operations using built-in LSPs.
* [ryan-WORK/ohm](https://github.com/ryan-WORK/ohm) ⭐ 17 | 🐛 2 | 🌐 Go | 📅 2026-08-01 - A persistent LSP process manager daemon which fixes memory bloat, stuck diagnostics, monorepo server duplication, and session degradation.
* [SunnyTamang/neodoc.nvim](https://github.com/SunnyTamang/neodoc.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2025-06-26 - DocString generator that helps writing function/classes docstrings in formats like `google`, `numpy`, `sphinx` with live preview.
* [idanarye/nvim-buffls](https://github.com/idanarye/nvim-buffls) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2026-05-10 - Add LSP functionality to specific buffers.
* [akioweh/lsp-document-highlight.nvim](https://github.com/akioweh/lsp-document-highlight.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-04-27 - Instantaneous LSP symbol reference highlighting under the cursor.
* [Senal-D-A-Gunaratna/swapson.nvim](https://github.com/Senal-D-A-Gunaratna/swapson.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - Monkeypatches `mason.nvim` to route `npm` and `pip` installs through `bun` and `uv`, speeding up LSP and tool installation.
* [\~chinmay/clangd\_extensions.nvim](https://sr.ht/~chinmay/clangd_extensions.nvim) - Off-spec `clangd` features for the built-in LSP client.

### Diagnostics

* [folke/trouble.nvim](https://github.com/folke/trouble.nvim) ⭐ 6,877 | 🐛 19 | 🌐 Lua | 📅 2025-10-31 - A pretty diagnostics list to help you solve all the trouble your code is causing.
* [piersolenski/wtf.nvim](https://github.com/piersolenski/wtf.nvim) ⭐ 607 | 🐛 0 | 🌐 Lua | 📅 2026-06-02 - AI powered diagnostic debugging, helps explain complex errors and offers custom tailored solutions.
* [artemave/workspace-diagnostics.nvim](https://github.com/artemave/workspace-diagnostics.nvim) ⭐ 259 | 🐛 2 | 🌐 Lua | 📅 2026-05-04 - Populate diagnostics for all projects files, not just the opened ones.
* [chrisgrieser/nvim-rulebook](https://github.com/chrisgrieser/nvim-rulebook) ⭐ 118 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Add inline-comments to ignore rules, or lookup rule documentation online.
* [sontungexpt/better-diagnostic-virtual-text](https://github.com/sontungexpt/better-diagnostic-virtual-text) ⭐ 94 | 🐛 3 | 🌐 Lua | 📅 2024-07-27 - Enhances the display of virtual text for diagnostics. This function aims to provide a more user-friendly and informative presentation of diagnostic messages directly within the editor.
* [Kurama622/clean-diagnostic](https://github.com/Kurama622/clean-diagnostic) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-04-29 - Display diagnostic count using virtual text, and show diagnostic details in a floating window.
* [tumillanino/semgrep.nvim](https://github.com/tumillanino/semgrep.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-06-27 - Lightweight Semgrep static analysis integration to catch bugs and vulnerabilities.
* [\~whynothugo/lsp\_lines.nvim](https://git.sr.ht/~whynothugo/lsp_lines.nvim) - Render diagnostics using virtual lines on top of the real line of code.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Completion

* [hrsh7th/nvim-cmp](https://github.com/hrsh7th/nvim-cmp) ⭐ 9,479 | 🐛 302 | 🌐 Lua | 📅 2026-07-09 - Completion engine written in Lua, successor of `nvim-compe`.
  * [hrsh7th/cmp-nvim-lsp](https://github.com/hrsh7th/cmp-nvim-lsp) ⭐ 1,510 | 🐛 29 | 🌐 Lua | 📅 2025-11-13 - `nvim-cmp` source for the built-in LSP client.
  * [saadparwaiz1/cmp\_luasnip](https://github.com/saadparwaiz1/cmp_luasnip) ⭐ 775 | 🐛 11 | 🌐 Lua | 📅 2024-11-04 - `nvim-cmp` source for `LuaSnip`.
  * [hrsh7th/cmp-path](https://github.com/hrsh7th/cmp-path) ⭐ 691 | 🐛 39 | 🌐 Lua | 📅 2025-07-30 - `nvim-cmp` source for filesystem paths.
  * [hrsh7th/cmp-nvim-lsp-signature-help](https://github.com/hrsh7th/cmp-nvim-lsp-signature-help) ⭐ 679 | 🐛 30 | 🌐 Lua | 📅 2025-11-14 - `nvim-cmp` source for displaying function signatures from an LSP client.
  * [hrsh7th/cmp-buffer](https://github.com/hrsh7th/cmp-buffer) ⭐ 669 | 🐛 38 | 🌐 Lua | 📅 2025-04-01 - `nvim-cmp` source for buffer words.
  * [hrsh7th/cmp-cmdline](https://github.com/hrsh7th/cmp-cmdline) ⭐ 620 | 🐛 66 | 🌐 Lua | 📅 2025-05-18 - `nvim-cmp` source for cmdline completion.
  * [petertriho/cmp-git](https://github.com/petertriho/cmp-git) ⭐ 420 | 🐛 12 | 🌐 Lua | 📅 2026-05-19 - `nvim-cmp` source for `git`.
  * [hrsh7th/cmp-nvim-lua](https://github.com/hrsh7th/cmp-nvim-lua) ⭐ 323 | 🐛 3 | 🌐 Lua | 📅 2025-11-14 - `nvim-cmp` source for the Neovim Lua API.
  * [lukas-reineke/cmp-under-comparator](https://github.com/lukas-reineke/cmp-under-comparator) ⭐ 193 | 🐛 0 | 🌐 Lua | 📅 2022-03-04 - `nvim-cmp` function for better sorting.
  * [SergioRibera/cmp-dotenv](https://github.com/SergioRibera/cmp-dotenv) ⭐ 93 | 🐛 3 | 🌐 Lua | 📅 2024-06-05 - `nvim-cmp` source for environment variables (from system and `.env` files).
  * [valenyala/cmp-forge-remappings](https://github.com/valenyala/cmp-forge-remappings) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2026-07-17 - `nvim-cmp` source for Solidity imports in Foundry projects, with remapping-aware paths and symbol auto-import.
* [nvim-mini/mini.nvim#mini.completion](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-completion.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for asynchronous two-stage completion. Supports showing completion item info and independent function signature.
* [saghen/blink.cmp](https://github.com/saghen/blink.cmp) ⭐ 6,516 | 🐛 99 | 🌐 Lua | 📅 2026-08-15 - Really fast completion with LSP and snippet support, along with signature help, cmdline completion, and autobracket support (based on semantic tokens).
  * [saghen/blink.compat](https://github.com/saghen/blink.compat) ⭐ 220 | 🐛 6 | 🌐 Lua | 📅 2025-05-28 - Compatibility layer for using `nvim-cmp` sources on `blink.cmp`.
  * [mikavilpas/blink-ripgrep.nvim](https://github.com/mikavilpas/blink-ripgrep.nvim) ⭐ 118 | 🐛 1 | 🌐 Lua | 📅 2026-08-13 - `blink.cmp` source for `ripgrep` / `git grep`.
  * [Kasier-Yang/blink-cmp-avante](https://github.com/Kaiser-Yang/blink-cmp-avante) ⭐ 114 | 🐛 3 | 🌐 Lua | 📅 2025-07-24 - `blink-cmp` source for Avante.
  * [Kaiser-Yang/blink-cmp-git](https://github.com/Kaiser-Yang/blink-cmp-git) ⭐ 91 | 🐛 6 | 🌐 Lua | 📅 2026-05-28 - `blink.cmp` source for Git.
  * [moyiz/blink-emoji.nvim](https://github.com/moyiz/blink-emoji.nvim) ⭐ 83 | 🐛 3 | 🌐 Lua | 📅 2026-04-11 - `blink.cmp` source for GitHub Markdown emojis.
  * [xieyonn/blink-cmp-dat-word](https://github.com/xieyonn/blink-cmp-dat-word) ⭐ 39 | 🐛 0 | 🌐 Lua | 📅 2026-02-13 - `blink.cmp` source for dictionary.
  * [disrupted/blink-cmp-conventional-commits](https://github.com/disrupted/blink-cmp-conventional-commits) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2026-04-20 - `blink.cmp` source for [Conventional Commits](https://www.conventionalcommits.org/).
  * [bydlw98/blink-cmp-env](https://github.com/bydlw98/blink-cmp-env) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-05-05 - `blink.cmp` source for environment variables.
  * [erooke/blink-cmp-latex](https://github.com/erooke/blink-cmp-latex) ⭐ 21 | 🐛 1 | 🌐 Lua | 📅 2026-04-09 - `blink.cmp` source for LaTeX.
  * [mgalliou/blink-cmp-tmux](https://github.com/mgalliou/blink-cmp-tmux) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-07-16 - `blink.cmp` source for [tmux](https://github.com/tmux/tmux) ⭐ 48,655 | 🐛 50 | 🌐 C | 📅 2026-08-15.
  * [krissen/blink-cmp-bibtex](https://github.com/krissen/blink-cmp-bibtex) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2026-08-14 - `blink.cmp` source for BibTeX citation files.
  * [bydlw98/blink-cmp-sshconfig](https://github.com/bydlw98/blink-cmp-sshconfig) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-05-03 - `blink.cmp` source for `sshconfig` files.
  * [benborla/at-file.nvim](https://github.com/benborla/at-file.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-05-23 - `blink.cmp` source for file path completion using `@`.
  * [yaocccc/blink-cmp-cmdlinehistory](https://github.com/yaocccc/blink-cmp-cmdlinehistory) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-03-26 - `blink.cmp` source for cmdline and search history.
  * [FelipeLema/blink-cmp-vsnip](https://codeberg.org/FelipeLema/blink-cmp-vsnip) - `blink.cmp` source for `vim-vsnip`.
* [zbirenbaum/copilot.lua](https://github.com/zbirenbaum/copilot.lua) ⭐ 4,093 | 🐛 21 | 🌐 Lua | 📅 2026-08-08 - Fully featured Lua replacement for [GitHub/copilot.vim](https://github.com/github/copilot.vim) ⭐ 11,676 | 🐛 63 | 🌐 Vim Script | 📅 2026-08-11.
* [ms-jpq/coq\_nvim](https://github.com/ms-jpq/coq_nvim) ⭐ 3,816 | 🐛 187 | 🌐 Lua | 📅 2026-08-10 - Fast as FUCK completion. SQLite, concurrent scheduler, hundreds of hours of optimization.
* [brianaung/compl.nvim](https://github.com/brianaung/compl.nvim) ⭐ 51 | 🐛 0 | 🌐 Lua | 📅 2026-04-27 - A minimal and dependency-free auto-completion built on top of Vim's ins-completion mechanism.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## AI

* [yetone/avante.nvim](https://github.com/yetone/avante.nvim) ⭐ 18,111 | 🐛 44 | 🌐 Lua | 📅 2026-08-16 - Chat with your code as if you are in Cursor AI IDE.
* [olimorris/codecompanion.nvim](https://github.com/olimorris/codecompanion.nvim) ⭐ 6,802 | 🐛 16 | 🌐 Lua | 📅 2026-08-12 - Copilot Chat like experience, complete with inline assistant. Supports Anthropic, Gemini, Ollama and OpenAI.
* [jackMort/ChatGPT.nvim](https://github.com/jackMort/ChatGPT.nvim) ⭐ 3,997 | 🐛 111 | 🌐 Lua | 📅 2026-01-13 - Effortless Natural Language Generation with OpenAI's ChatGPT API.
* [nickjvandyke/opencode.nvim](https://github.com/nickjvandyke/opencode.nvim) ⭐ 3,777 | 🐛 5 | 🌐 Lua | 📅 2026-07-30 - OpenCode AI assistant integration.
* [CopilotC-Nvim/CopilotChat.nvim](https://github.com/CopilotC-Nvim/CopilotChat.nvim) ⭐ 3,650 | 🐛 22 | 🌐 Lua | 📅 2026-08-03 - A chat interface for GitHub Copilot that allows you to directly ask and receive answers to coding-related questions.
* [David-Kunz/gen.nvim](https://github.com/David-Kunz/gen.nvim) ⭐ 1,528 | 🐛 26 | 🌐 Lua | 📅 2025-05-03 - Generate text using LLMs (via Ollama) with customizable prompts.
* [milanglacier/minuet-ai.nvim](https://github.com/milanglacier/minuet-ai.nvim) ⭐ 1,369 | 🐛 12 | 🌐 Lua | 📅 2026-08-14 - Minuet offers code completion from LLM providers including OpenAI (compatible), Gemini, Claude, Ollama, Deepseek and more providers, with support for nvim-cmp, blink.cmp and virtual-text frontend.
* [Robitx/gp.nvim](https://github.com/Robitx/gp.nvim) ⭐ 1,321 | 🐛 68 | 🌐 Lua | 📅 2025-08-11 - ChatGPT like sessions and instructable text/code operations in your favorite editor.
* [Exafunction/windsurf.nvim](https://github.com/Exafunction/windsurf.nvim) ⭐ 1,289 | 🐛 115 | 🌐 Lua | 📅 2026-04-02 - Free, ultrafast Copilot alternative. Supports LSP and Tree-sitter.
* [Davidyz/VectorCode](https://github.com/davidyz/vectorcode) ⭐ 871 | 🐛 18 | 🌐 Python | 📅 2026-02-23 - Supercharge your LLM experience with repository-level RAG.
* [carlos-algms/agentic.nvim](https://github.com/carlos-algms/agentic.nvim) ⭐ 589 | 🐛 15 | 🌐 Lua | 📅 2026-08-10 - Chat interface for AI ACP providers such as Claude, Gemini, Codex, OpenCode and Cursor.
* [dense-analysis/neural](https://github.com/dense-analysis/neural) ⭐ 512 | 🐛 18 | 🌐 Vim Script | 📅 2025-07-22 - Integrate LLMs for generating code, interacting with chat bots, and more.
* [Kurama622/llm.nvim](https://github.com/Kurama622/llm.nvim) ⭐ 478 | 🐛 0 | 🌐 Lua | 📅 2026-06-20 - Free large language model (LLM) support, provides commands to interact with LLM.
* [dlants/magenta.nvim](https://github.com/dlants/magenta.nvim) ⭐ 462 | 🐛 14 | 🌐 TypeScript | 📅 2026-08-08 - Leverage coding assistants for chat and code generation. Provides tools for the AI/LLM agent to explore and edit your code, like Aider, Cursor and Windsurf.
* [gsuuon/model.nvim](https://github.com/gsuuon/model.nvim) ⭐ 398 | 🐛 15 | 🌐 Lua | 📅 2025-07-23 - Integrate LLMs via a prompt builder interface. Multi-providers including OpenAI (+ compatibles), `PaLM`, `Hugging Face`, and local engines like `llamacpp`.
* [GeorgesAlkhouri/nvim-aider](https://github.com/GeorgesAlkhouri/nvim-aider) ⭐ 377 | 🐛 6 | 🌐 Lua | 📅 2026-08-03 - Seamlessly integrate Aider for an AI-assisted coding experience.
* [azorng/goose.nvim](https://github.com/azorng/goose.nvim) ⭐ 315 | 🐛 6 | 🌐 Lua | 📅 2026-04-16 - Seamless integration with [goose](https://block.github.io/goose) - work with a powerful AI agent without leaving your editor.
* [tzachar/cmp-ai](https://github.com/tzachar/cmp-ai) ⭐ 276 | 🐛 5 | 🌐 Lua | 📅 2026-02-08 - This is a general purpose AI source for nvim-cmp, easily adapted to any REST API supporting remote code completion.
* [jpmcb/nvim-llama](https://github.com/jpmcb/nvim-llama) ⭐ 272 | 🐛 9 | 🌐 Python | 📅 2025-03-09 - LLM (LLaMA 2 and `llama.cpp`) wrappers.
* [kiddos/gemini.nvim](https://github.com/kiddos/gemini.nvim) ⭐ 261 | 🐛 11 | 🌐 Lua | 📅 2026-06-19 - Bindings to Google Gemini API.
* [milanglacier/yarepl.nvim#aider-extensions](https://github.com/milanglacier/yarepl.nvim/blob/main/extensions/README.md) ⭐ 251 | 🐛 2 | 🌐 Lua | 📅 2026-08-02 - Integration with [aider-chat](https://aider.chat), a TUI AI coding assistant.
* [cursortab/cursortab.nvim](https://github.com/cursortab/cursortab.nvim) ⭐ 244 | 🐛 5 | 🌐 Go | 📅 2026-08-05 - Edit completions and cursor predictions with multiple AI providers.
* [mozanunal/sllm.nvim](https://github.com/mozanunal/sllm.nvim) ⭐ 113 | 🐛 11 | 🌐 Lua | 📅 2026-02-08 - In-editor chat powered by Simon Willison's LLM CLI: stream replies in a Markdown buffer, manage rich context (files, URLs, selections, diagnostics, shell outputs), switch models interactively, and even see token-usage stats.
* [Aaronik/GPTModels.nvim](https://github.com/Aaronik/GPTModels.nvim) ⭐ 74 | 🐛 2 | 🌐 Lua | 📅 2025-06-26 - GPTModels - a stable, clean, multi model, window based LLM AI tool.
* [teocns/neocursor.nvim](https://github.com/teocns/neocursor.nvim) ⭐ 59 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Next-edit predictions, cursor jumps, and ghost text, all driven by an existing Cursor session instead of an API key.
* [Flemma-Dev/flemma.nvim](https://github.com/Flemma-Dev/flemma.nvim) ⭐ 57 | 🐛 1 | 🌐 Lua | 📅 2026-07-29 - Turn messy inputs (meeting transcripts, briefs, PDFs, email threads) into polished documents, iterate over many turns, and get a second opinion from a different model on the same draft, stored in a `.chat` file.
* [CamdenClark/flyboy](https://github.com/CamdenClark/flyboy) ⭐ 46 | 🐛 1 | 🌐 Lua | 📅 2023-10-31 - Simple interaction with ChatGPT in a Markdown buffer. Supports GPT-4 and Azure OpenAI.
* [ishiooon/codex.nvim](https://github.com/ishiooon/codex.nvim) ⭐ 37 | 🐛 1 | 🌐 Lua | 📅 2026-06-18 - Codex IDE integration, no API key required.
* [you-n-g/simplegpt.nvim](https://github.com/you-n-g/simplegpt.nvim) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2026-04-13 - Provide a simple yet flexible way to construct and send questions to ChatGPT.
* [taigrr/neocrush.nvim](https://github.com/taigrr/neocrush.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-08-02 - Integration with Crush AI coding assistant, with edit highlighting, auto-focus, Telescope support, terminal and version management.
* [3v0k4/exit.nvim](https://github.com/3v0k4/exit.nvim) ⭐ 18 | 🐛 3 | 🌐 Lua | 📅 2024-12-19 - Prompt LLMs (large language models) to write Vim commands.
* [k2589/LLuMinate.nvim](https://github.com/k2589/lluminate.nvim) ⭐ 17 | 🐛 1 | 🌐 Lua | 📅 2024-10-11 - Enrich context for LLM with LSP hover added to clipboard.
* [ray-x/copilot-agent.nvim](https://github.com/ray-x/copilot-agent.nvim) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2026-06-03 - GitHub Copilot agent runtime with native tool execution, session persistence, and fine-grained permissions.
* [zgs225/pi2.nvim](https://github.com/zgs225/pi2.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-08-14 - Frontend for the [pi](https://pi.dev) coding agent with in-editor chat, reviewed diffs, session-tree navigation, and extension prompts.
* [chatvim/chatvim.nvim](https://github.com/chatvim/chatvim.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-10-02 - Chat with Markdown files using AI models from xAI, OpenAI and Anthropic.
* [BRONZowl/codux.nvim](https://github.com/BRONZowl/codux.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-07-15 - Run OpenAI Codex in a persistent floating terminal and send files, selections, diagnostics, or file explorer targets.
* [heilgar/nochat.nvim](https://github.com/heilgar/nochat.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-03-13 - Cursor-like effortless natural language generation with multiple AI providers including Ollama, Anthropic (Claude), and ChatGPT.
* [blob42/codegpt-ng.nvim](https://github.com/blob42/codegpt-ng.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-05-12 - Minimalist command based AI coding with a powerful template system. Supports Ollama, OpenAI and more.
* [ctchen222/openspec.nvim](https://github.com/ctchen222/openspec.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - OpenSpec workflow context, model/provider selection, and coding-agent implementation handoffs.
* [0xble/dotagent.nvim](https://github.com/0xble/dotagent.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-04-26 - Command and skill completion for Claude Code and Codex-style prompt editors, configurable from local agent command and skill directories.
* [julwrites/llm-nvim](https://github.com/julwrites/llm-nvim) ⭐ 9 | 🐛 4 | 🌐 Lua | 📅 2026-08-15 - Comprehensive integration with the [LLM](https://github.com/simonw/llm) ⭐ 12,366 | 🐛 679 | 🌐 Python | 📅 2026-08-12 tool.
* [3ZsForInsomnia/code-companion-picker](https://github.com/3ZsForInsomnia/code-companion-picker) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2026-03-24 - Snacks picker integrations for previewing CodeCompanion prompts and Skills (using OpenSkills).
* [3ZsForInsomnia/token-count.nvim](https://github.com/3ZsForInsomnia/token-count.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-06-06 - Shows the token count for the current buffer, with integrations for Lualine and NeoTree.
* [wsdjeg/chat.nvim](https://github.com/wsdjeg/chat.nvim) ⭐ 7 | 🐛 2 | 🌐 Lua | 📅 2026-08-16 - A lightweight, extensible chat plugin with AI integration, multiple providers, and built-in tools.
* [nishu-murmu/cursor-inline](https://github.com/nishu-murmu/cursor-inline) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-08-05 - Cursor-style inline AI editing. Select code, describe the change, and get an inline, highlighted edit you can accept or reject—similar to Cursor inline workflow.
* [alsi-lawr/agent-term.nvim](https://github.com/alsi-lawr/agent-term.nvim) ⭐ 7 | 🐛 5 | 🌐 Lua | 📅 2026-07-23 - Terminal-agent UI with persistent views, lightweight hook-based editor context, and extensible presets for any native AI TUI.
* [3ZsForInsomnia/vs-code-companion](https://github.com/3ZsForInsomnia/vs-code-companion) ⭐ 6 | 🐛 3 | 🌐 Lua | 📅 2025-10-22 - Tool for importing VSCode's Markdown prompts into CodeCompanion.
* [nwiizo/signalbox.nvim](https://github.com/nwiizo/signalbox.nvim) ⭐ 4 | 🐛 1 | 🌐 Lua | 📅 2026-08-13 - Attention-first control surface for monitoring and routing persistent Herdr coding agents.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Programming Languages Support

* [nvim-java/nvim-java](https://github.com/nvim-java/nvim-java) ⭐ 1,689 | 🐛 36 | 🌐 Lua | 📅 2026-07-04 - Everything you need for a painless Java experience.
* [nvim-flutter/flutter-tools.nvim](https://github.com/nvim-flutter/flutter-tools.nvim) ⭐ 1,398 | 🐛 29 | 🌐 Lua | 📅 2026-08-06 - Build Flutter and Dart applications using the native LSP.
* [chomosuke/typst-preview.nvim](https://github.com/chomosuke/typst-preview.nvim) ⭐ 985 | 🐛 13 | 🌐 Lua | 📅 2026-07-14 - Preview Typst documents in the browser, instant update on each keystroke, and cross jump between code and preview.
* [Julian/lean.nvim](https://github.com/Julian/lean.nvim) ⭐ 563 | 🐛 37 | 🌐 Lua | 📅 2026-08-10 - Support for the [Lean Theorem Prover](https://leanprover.github.io/).
* [dmmulroy/tsc.nvim](https://github.com/dmmulroy/tsc.nvim) ⭐ 547 | 🐛 7 | 🌐 Lua | 📅 2026-01-14 - Asynchronous project-wide TypeScript type-checking using the TypeScript compiler (`tsc`) with results loaded into a quickfix list.
* [quarto-dev/quarto-nvim](https://github.com/quarto-dev/quarto-nvim) ⭐ 530 | 🐛 6 | 🌐 Lua | 📅 2026-04-22 - Tools for working with [Quarto](https://quarto.org/) documents.
* [dmmulroy/ts-error-translator.nvim](https://github.com/dmmulroy/ts-error-translator.nvim) ⭐ 434 | 🐛 2 | 🌐 Lua | 📅 2026-01-03 - A port of Matt Pocock's `ts-error-translator` for VSCode for turning messy and confusing TypeScript errors into plain English.
* [gennaro-tedesco/nvim-jqx](https://github.com/gennaro-tedesco/nvim-jqx) ⭐ 338 | 🐛 2 | 🌐 Lua | 📅 2024-05-31 - Interactive interface for JSON files.
* [iabdelkareem/csharp.nvim](https://github.com/iabdelkareem/csharp.nvim) ⭐ 273 | 🐛 14 | 🌐 Lua | 📅 2024-08-25 - Enhances the development experience for .NET developers.
* [nanotee/sqls.nvim](https://github.com/nanotee/sqls.nvim) ⭐ 258 | 🐛 10 | 🌐 Lua | 📅 2026-08-13 - SQL database connection plugin + LSP client.
* [AckslD/swenv.nvim](https://github.com/AckslD/swenv.nvim) ⭐ 252 | 🐛 12 | 🌐 Lua | 📅 2025-02-09 - Tiny plugin to quickly switch Python virtual environments without restarting.
* [apyra/nvim-unity.nvim](https://github.com/apyra/nvim-unity) ⭐ 123 | 🐛 11 | 🌐 C# | 📅 2026-04-01 - Editor support for Unity with full LSP support via OmniSharp.
* [gbprod/phpactor.nvim](https://github.com/gbprod/phpactor.nvim) ⭐ 98 | 🐛 2 | 🌐 Lua | 📅 2026-01-07 - Lua version of [phpactor](https://github.com/phpactor/phpactor) ⭐ 1,916 | 🐛 294 | 🌐 PHP | 📅 2026-08-15.
* [TheLeoP/powershell.nvim](https://github.com/TheLeoP/powershell.nvim) ⭐ 82 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - First class PowerShell editor integration. Includes LSP, debugging (requires nvim-dap) and $psEditor API support.
* [kiyoon/python-import.nvim](https://github.com/kiyoon/python-import.nvim) ⭐ 62 | 🐛 0 | 🌐 Python | 📅 2025-08-12 - Add Python import statements with Tree-sitter, LSP, and more.
* [J-Cowsert/classlayout.nvim](https://github.com/J-Cowsert/classlayout.nvim) ⭐ 60 | 🐛 3 | 🌐 Lua | 📅 2026-04-17 - Visualize C/C++ struct and class memory layouts (field offsets, padding, alignment) in a floating window.
* [artur-shaik/jc.nvim](https://github.com/artur-shaik/jc.nvim) ⭐ 59 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - Java productivity layer on top of an externally managed `jdtls`, including class creation, code generation, annotation by search, refactoring, a neotest test runner, and a task runner for `gradle` and `maven`.
* [niuiic/typst-preview.nvim](https://github.com/niuiic/typst-preview.nvim) ⭐ 49 | 🐛 1 | 🌐 Lua | 📅 2025-05-19 - Preview Typst documents, respond to file changes.
* [neolooong/whichpy.nvim](https://github.com/neolooong/whichpy.nvim) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2026-05-09 - Switch Python interpreter without restarting LSP.
* [atomicptr/defold.nvim](https://github.com/atomicptr/defold.nvim) ⭐ 34 | 🐛 11 | 🌐 Rust | 📅 2026-08-10 - Batteries-included development environment for the Defold game engine.
* [kiyoon/haskell-scope-highlighting.nvim](https://github.com/kiyoon/haskell-scope-highlighting.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2025-12-20 - Haskell syntax highlighting which considers variable scopes. Inspired from "Context Coloring" by prof. Douglas Crockford.
* [alessio-vivaldelli/java-creator-nvim](https://github.com/alessio-vivaldelli/java-creator-nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2026-02-07 - Interactive Java file creator with automatic package detection, supporting classes, interfaces, enums, records and abstract classes.
* [brendalf/mix.nvim](https://github.com/brendalf/mix.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2022-08-22 - Mix (from Elixir) wrapper plugin.
* [sachinsenal0x64/hot.nvim](https://github.com/sachinsenal0x64/hot.nvim) ⚠️ Archived - A hot reloader that works with any programming language.
* [ta-tikoma/php.easy.nvim](https://github.com/ta-tikoma/php.easy.nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2026-02-25 - Methods of assistance in PHP development: create classes, constants, methods, properties; simple copying and deleting of an entity.
* [simonwinther/cppman.nvim](https://github.com/simonwinther/cppman.nvim) ⭐ 23 | 🐛 2 | 🌐 Lua | 📅 2026-06-24 - Search C++ docs from cppman and view results in a floating window, backed by a local SQLite index for fast lookups.
* [mosheavni/yaml-companion.nvim](https://github.com/mosheavni/yaml-companion.nvim) ⭐ 20 | 🐛 1 | 🌐 Lua | 📅 2026-07-14 - Automatic schema detection and selection for YAML files with `yaml-language-server`, including built-in Kubernetes support.
* [leblocks/hopcsharp.nvim](https://github.com/leblocks/hopcsharp.nvim) ⭐ 17 | 🐛 9 | 🌐 Lua | 📅 2026-08-13 - Provides LSP-less navigation and type-hierarchy information in C# repositories.
* [onlyati/quadlet-lsp.nvim](https://github.com/onlyati/quadlet-lsp.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2025-12-10 - Provides completion, hover and other language server features for Podman Quadlet files.
* [Who5673/who5673-nasm](https://github.com/Who5673/who5673-nasm) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - Helps people program Netwide Assembler language faster and more convenient using snippets.
* [chuwy/ucm.nvim](https://github.com/chuwy/ucm.nvim) ⭐ 6 | 🐛 2 | 🌐 Lua | 📅 2023-08-23 - Navigating [Unison](https://unison-lang.org/) projects.
* [AnsonH/copy-python-path.nvim](https://github.com/AnsonH/copy-python-path.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-07-01 - Copy the reference or import path of a Python symbol.
* [redpierrot/ballerina.nvim](https://github.com/redpierrot/ballerina.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-07-23 - Syntax highlighting, LSP, debugging, package-aware format-on-save, auto-indent, and `bal` run/test/build commands for the Ballerina language.
* [clang-engineer/jvm-env.nvim](https://github.com/clang-engineer/jvm-env.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-07-20 - Auto-detects installed JDKs by major version, with separate environment variables for jdtls and Gradle.
* [awsum-lang/awsum-nvim](https://github.com/awsum-lang/awsum-nvim) ⭐ 4 | 🐛 0 | 🌐 C | 📅 2026-06-22 - LSP client and Tree-sitter highlighting for the [Awsum](https://awsum-lang.org) programming language.
* [cuducos.me/yaml.nvim](https://tangled.org/cuducos.me/yaml.nvim) - Utils to work with YAML files.

### Golang

* [ray-x/go.nvim](https://github.com/ray-x/go.nvim) ⭐ 2,652 | 🐛 96 | 🌐 Lua | 📅 2026-06-04 - Golang plugin based on LSP and Tree-sitter.
* [olexsmir/gopher.nvim](https://github.com/olexsmir/gopher.nvim/) ⭐ 434 | 🐛 6 | 🌐 Lua | 📅 2026-07-12 - Plugin for making Golang development easiest.
* [fredrikaverpil/godoc.nvim](https://github.com/fredrikaverpil/godoc.nvim) ⭐ 175 | 🐛 4 | 🌐 Lua | 📅 2026-08-01 - Fuzzy search Go packages/symbols and view docs.
* [crispgm/nvim-go](https://github.com/crispgm/nvim-go) ⭐ 155 | 🐛 3 | 🌐 Lua | 📅 2026-04-01 - A minimal implementation of Golang development plugin.
* [maxandron/goplements.nvim](https://github.com/maxandron/goplements.nvim) ⭐ 90 | 🐛 4 | 🌐 Lua | 📅 2025-12-15 - Visualize Go struct and interface implementations.
* [rafaelsq/nvim-goc.lua](https://github.com/rafaelsq/nvim-goc.lua) ⭐ 55 | 🐛 0 | 🌐 Lua | 📅 2025-11-14 - Highlight your buffer with Golang Code Coverage.
* [crusj/structrue-go.nvim](https://github.com/crusj/structrue-go.nvim) ⭐ 48 | 🐛 1 | 🌐 Lua | 📅 2022-09-29 - A better structured display of Golang symbols information.
* [crusj/hierarchy-tree-go.nvim](https://github.com/crusj/hierarchy-tree-go.nvim) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2022-12-01 - Golang integration with `callHierarchy` UI tree.
* [Snikimonkd/cmp-go-pkgs](https://github.com/Snikimonkd/cmp-go-pkgs) ⭐ 31 | 🐛 3 | 🌐 Lua | 📅 2025-01-07 - Cmp source for Go packages names.
* [yanskun/gotests.nvim](https://github.com/yanskun/gotests.nvim) ⭐ 29 | 🐛 1 | 🌐 Lua | 📅 2024-07-11 - Make Go tests easy with [gotests](https://github.com/cweill/gotests) ⭐ 5,327 | 🐛 39 | 🌐 Go | 📅 2025-10-30.
* [romus204/go-tagger.nvim](https://github.com/romus204/go-tagger.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - A lightweight plugin to manage struct field tags in Go files.
* [sjclayton/goplexity.nvim](https://github.com/sjclayton/goplexity.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-04-09 - Time/space (Big-O) complexity analyzer for Golang.
* [Yu-Leo/gosigns.nvim](https://github.com/Yu-Leo/gosigns.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-03-08 - Visualize some Go hints: struct, interface, and methods implementations; go comments.
* [Yu-Leo/cmp-go-pkgs](https://github.com/Yu-Leo/cmp-go-pkgs) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-03-04 - Cmp source providing the names of Go packages to import.

### Web Development

* [mistweaverco/kulala.nvim](https://github.com/mistweaverco/kulala.nvim) ⭐ 2,143 | 🐛 6 | 🌐 Lua | 📅 2026-08-12 - A minimal HTTP-client interface.
* [rest-nvim/rest.nvim](https://github.com/rest-nvim/rest.nvim) ⭐ 2,048 | 🐛 46 | 🌐 Lua | 📅 2025-12-27 - A fast HTTP client written in Lua.
* [yelog/i18n.nvim](https://github.com/yelog/i18n.nvim) ⭐ 62 | 🐛 0 | 🌐 Lua | 📅 2026-08-06 - Internationalization (i18n) management with LSP support for `Vue`, `React`, `Java` and more.
* [cjodo/convert.nvim](https://github.com/cjodo/convert.nvim) ⭐ 58 | 🐛 0 | 🌐 Lua | 📅 2026-01-16 - Helps with CSS unit conversions.
* [lima1909/resty.nvim](https://github.com/lima1909/resty.nvim) ⭐ 53 | 🐛 2 | 🌐 Lua | 📅 2026-04-27 - Fast and easy-to-use HTTP-Rest-Client.
* [mawkler/jsx-element.nvim](https://github.com/mawkler/jsx-element.nvim) ⭐ 28 | 🐛 1 | 🌐 Lua | 📅 2026-07-20 - JSX/TSX text-objects and motions.
* [Kenzo-Wada/boundary.nvim](https://github.com/Kenzo-Wada/boundary.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2025-10-28 - Display `'use client'` markers inline in your JSX code to visualize client component boundaries.
* [heilgar/nvim-http-client](https://github.com/heilgar/nvim-http-client) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2025-10-06 - Easy to use HTTP client with IntelliJ (JetBrains) HTTP client syntax compatibility.
* [abidibo/nvim-httpyac](https://github.com/abidibo/nvim-httpyac) ⭐ 18 | 🐛 1 | 🌐 Lua | 📅 2026-04-18 - Provides integration with `httpYac`.
* [BibekBhusal0/nvim-shadcn](https://github.com/BibekBhusal0/nvim-shadcn) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-02-14 - Easily add Shadcn UI components with telescope.
* [ankushbhagats/liveserver.nvim](https://github.com/ankushbhagats/liveserver.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-04-11 - Live-server integration with smart commands and a clickable lualine toggle.
* [farias-hecdin/CSSVarViewer](https://github.com/farias-hecdin/CSSVarViewer) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2024-10-01 - Easily visualize the content of your CSS variables in a virtual text.
* [rodrigoscc/nurl.nvim](https://github.com/rodrigoscc/nurl.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-05-18 - HTTP client with requests defined in pure Lua.
* [farias-hecdin/CSSVarHighlight](https://github.com/farias-hecdin/CSSVarHighlight) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2024-09-24 - Quickly highlight the color you defined in your CSS variables with the help of `mini.hipatterns`.
* [harukikuri/viteenv.nvim](https://github.com/harukikuri/viteenv.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-07-02 - Shows the effective value of `import.meta.env` variables inline per mode, resolved by your project's own `Vite`.
* [azratul/expose-localhost.nvim](https://github.com/azratul/expose-localhost.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-03-28 - Expose your local server to the internet with cloudflared or ngrok.
* [tednguyendev/recent\_rails.nvim](https://github.com/tednguyendev/recent_rails.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - Telescope picker for recent Rails actions, views, and errors.

### Markdown and LaTeX

* [iamcco/markdown-preview.nvim](https://github.com/iamcco/markdown-preview.nvim) ⭐ 7,959 | 🐛 264 | 🌐 JavaScript | 📅 2024-07-23 - Preview Markdown on your modern browser with synchronised scrolling and flexible configuration.
* [MeanderingProgrammer/render-markdown.nvim](https://github.com/MeanderingProgrammer/render-markdown.nvim) ⭐ 4,920 | 🐛 12 | 🌐 Lua | 📅 2026-08-11 - Improve viewing Markdown files directly.
* [OXY2DEV/markview.nvim](https://github.com/OXY2DEV/markview.nvim) ⭐ 3,597 | 🐛 4 | 🌐 Lua | 📅 2026-08-14 - A hackable Markdown, Typst, LaTeX, HTML (inline) and YAML renderer.
* [toppair/peek.nvim](https://github.com/toppair/peek.nvim) ⭐ 874 | 🐛 38 | 🌐 TypeScript | 📅 2024-08-20 - Preview Markdown in a webview window.
* [frabjous/knap](https://github.com/frabjous/knap) ⭐ 391 | 🐛 8 | 🌐 Lua | 📅 2024-10-22 - Plugin for creating automatic updating-as-you-type previews for Markdown, LaTeX and other documents.
* [kdheepak/panvimdoc](https://github.com/kdheepak/panvimdoc) ⭐ 323 | 🐛 6 | 🌐 CSS | 📅 2026-04-12 - A pandoc to vimdoc GitHub action.
* [YousefHadder/markdown-plus.nvim](https://github.com/YousefHadder/markdown-plus.nvim) ⭐ 285 | 🐛 10 | 🌐 Lua | 📅 2026-08-14 - Provides a full editing experience for Markdown files which includes support for lists, links, TOC, and more with simple and fast keymaps.
* [Zeioth/markmap.nvim](https://github.com/Zeioth/markmap.nvim) ⭐ 256 | 🐛 2 | 🌐 Lua | 📅 2025-11-11 - Visualize your Markdown as mindmaps.
* [tadmccorkle/markdown.nvim](https://github.com/tadmccorkle/markdown.nvim) ⭐ 249 | 🐛 9 | 🌐 Lua | 📅 2025-12-22 - Configurable tools for Markdown files, including inline-style, link, and navigation keymaps, table of contents, improved list editing, and more.
* [Thiago4532/mdmath.nvim](https://github.com/Thiago4532/mdmath.nvim) ⭐ 236 | 🐛 13 | 🌐 Lua | 📅 2024-12-27 - A Markdown equation previewer, using kitty Graphics Protocol.
* [jubnzv/mdeval.nvim](https://github.com/jubnzv/mdeval.nvim) ⭐ 230 | 🐛 4 | 🌐 Lua | 📅 2026-05-03 - Evaluate code blocks inside Markdown documents.
* [jghauser/follow-md-links.nvim](https://github.com/jghauser/follow-md-links.nvim) ⭐ 177 | 🐛 9 | 🌐 Lua | 📅 2026-02-24 - Press enter to follow internal Markdown links.
* [Myzel394/easytables.nvim](https://github.com/Myzel394/easytables.nvim) ⭐ 146 | 🐛 2 | 🌐 Lua | 📅 2025-11-02 - Easily insert and edit Markdown tables with a live preview and useful helpers.
* [nvim-telescope/telescope-bibtex.nvim](https://github.com/nvim-telescope/telescope-bibtex.nvim) ⭐ 134 | 🐛 16 | 🌐 Lua | 📅 2024-03-28 - Telescope extension to search and paste BibTeX entries into your TeX files.
* [davidgranstrom/nvim-markdown-preview](https://github.com/davidgranstrom/nvim-markdown-preview) ⭐ 112 | 🐛 11 | 🌐 CSS | 📅 2023-07-11 - Markdown preview in the browser using pandoc and live-server through the job-control API.
* [Kicamon/markdown-table-mode.nvim](https://github.com/Kicamon/markdown-table-mode.nvim) ⭐ 107 | 🐛 5 | 🌐 Lua | 📅 2026-04-22 - Markdown format plugin like vim-table-mode but write in Lua.
* [SCJangra/table-nvim](https://github.com/SCJangra/table-nvim) ⭐ 85 | 🐛 1 | 🌐 Lua | 📅 2026-03-12 - A Markdown table editor that formats the table as you type.
* [OXY2DEV/markdoc.nvim](https://github.com/OXY2DEV/markdoc.nvim) ⭐ 53 | 🐛 1 | 🌐 Lua | 📅 2025-11-14 - Tree-sitter based `markdown -> vimdoc` converter.
* [richardbizik/nvim-toc](https://github.com/richardbizik/nvim-toc) ⭐ 52 | 🐛 0 | 🌐 Lua | 📅 2026-01-06 - Easily generate table of contents for Markdown files.
* [mpas/marp-nvim](https://github.com/mpas/marp-nvim) ⭐ 51 | 🐛 0 | 🌐 Lua | 📅 2024-07-31 - Present using Markdown with [Marp](https://marp.app/).
* [jghauser/auto-pandoc.nvim](https://github.com/jghauser/auto-pandoc.nvim) ⭐ 41 | 🐛 1 | 🌐 Nix | 📅 2025-08-31 - Easy pandoc conversion leveraging YAML blocks.
* [kibi2/tirenvi.nvim](https://github.com/kibi2/tirenvi.nvim) ⭐ 39 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - Edit Markdown and CSV tables with lossless round-trip.
* [yaocccc/nvim-hl-mdcodeblock.lua](https://github.com/yaocccc/nvim-hl-mdcodeblock.lua) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2026-03-04 - Highlight Markdown codeblock using Tree-sitter.
* [Prgebish/sigil.nvim](https://github.com/Prgebish/sigil.nvim) ⭐ 35 | 🐛 1 | 🌐 Lua | 📅 2026-04-28 - Implementation of Emacs' `prettify-symbols-mode` to visually replace text patterns with Unicode symbols while editing LaTeX and Typst files.
* [Nedra1998/nvim-mdlink](https://github.com/Nedra1998/nvim-mdlink) ⭐ 33 | 🐛 1 | 🌐 Lua | 📅 2024-12-24 - Simplify creating and following Markdown links.
* [jbyuki/carrot.nvim](https://github.com/jbyuki/carrot.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2025-06-01 - Markdown evaluator Lua code blocks.
* [kiran94/edit-markdown-table.nvim](https://github.com/kiran94/edit-markdown-table.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2023-05-28 - Edit Markdown Tables using Tree-sitter.
* [nfrid/markdown-togglecheck](https://github.com/nfrid/markdown-togglecheck) ⭐ 23 | 🐛 1 | 🌐 Lua | 📅 2023-09-04 - Toggle task list check boxes using Tree-sitter.
* [timantipov/md-table-tidy.nvim](https://github.com/timantipov/md-table-tidy.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-08-12 - Simple Markdown tables formatting.
* [itsfernn/vimtex-follow](https://github.com/itsfernn/vimtex-follow) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Adds a toggleable "follow mode", synchronizing your PDF viewer with your cursor position.
* [ChuufMaster/markdown-toc](https://github.com/ChuufMaster/markdown-toc) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2025-05-28 - Generate TOC in any Markdown file from any other Markdown file with customisable levels of headings and affordances for emojis and ensuring that it works on GitHub using relative paths.
* [satozawa/graft.nvim](https://github.com/satozawa/graft.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-04-15 - Tree-structured editing for Markdown bullet lists with subtree text objects, Alt+hjkl navigation, and structural operations.
* [gunasekar/markview-smart-tables.nvim](https://github.com/gunasekar/markview-smart-tables.nvim) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2026-06-21 - Auto-fit and word-wrap wide Markdown tables in `markview.nvim`.
* [dominic-righthere/markdown-pipetable.nvim](https://github.com/dominic-righthere/markdown-pipetable.nvim) ⭐ 6 | 🐛 1 | 🌐 Lua | 📅 2026-07-17 - Interactive, fit-to-width inline Markdown table editor with cell navigation, visual selection, row/column operations, and CSV/TSV conversion.
* [tttol/md-outline.nvim](https://github.com/tttol/md-outline.nvim) ⭐ 5 | 🐛 3 | 🌐 Lua | 📅 2025-11-10 - Automatically displays an outline for Markdown files.
* [rogue-87/inlyne.nvim](https://github.com/rogue-87/inlyne.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-03-28 - Wrapper for [inlyne](https://github.com/Inlyne-Project/inlyne) ⭐ 1,335 | 🐛 64 | 🌐 Rust | 📅 2026-08-06 Markdown viewer.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Language

* [potamides/pantran.nvim](https://github.com/potamides/pantran.nvim) ⭐ 331 | 🐛 11 | 🌐 Lua | 📅 2025-04-07 - Translate your text with an interactive translation window.
* [niuiic/translate.nvim](https://github.com/niuiic/translate.nvim) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2024-11-17 - Invoke any translation engine via shell command.
* [kiyoon/Korean-IME.nvim](https://github.com/kiyoon/Korean-IME.nvim) ⭐ 40 | 🐛 1 | 🌐 Lua | 📅 2026-01-28 - OS-independent Korean input method that converts English inputs to Korean in-place.
* [bennorichters/taal.nvim](https://github.com/bennorichters/taal.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-05-16 - Improve grammar and spelling errors in multiple languages using LLMs.
* [sontungexpt/vietnamese.nvim](https://github.com/sontungexpt/vietnamese.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-06-11 - A Vietnamese input method engine with native support to type Vietnamese in insert mode.
* [noir4y/comment-translate.nvim](https://github.com/noir4y/comment-translate.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-07-03 - Translate code comments and strings using online as well as local LLMs or external translators.
* [acidsugarx/babel.nvim](https://github.com/acidsugarx/babel.nvim) ⭐ 14 | 🐛 2 | 🌐 Lua | 📅 2026-08-10 - Translate text using Google Translate with async support, float display, and multi-picker integration.
* [tanloong/interlaced.nvim](https://github.com/tanloong/interlaced.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-04-30 - Help align bilingual parallel texts.
* [walkersumida/deepl.nvim](https://github.com/walkersumida/deepl.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2025-11-22 - Translates text using the DeepL API with multiple output modes (float, replace, append).
* [doodleEsc/translator.nvim](https://github.com/doodleEsc/translator.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-09-01 - A powerful AI-powered translation plugin, leveraging OpenAI's GPT models to provide high-quality translations with natural language understanding.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Syntax

* [nvim-treesitter/nvim-treesitter](https://github.com/nvim-treesitter/nvim-treesitter) ⭐ 14,316 | 🐛 270 | 🌐 Tree-sitter Query | 📅 2026-08-15 - Tree-sitter configurations and abstraction layer.
* [nvim-mini/mini.nvim#mini.surround](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-surround.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for working with text surroundings (add, delete, replace, find, highlight). Supports dot-repeat, different search methods, "last"/"next" extended mappings, Tree-sitter integration, and more.
* [kylechui/nvim-surround](https://github.com/kylechui/nvim-surround) ⭐ 4,275 | 🐛 11 | 🌐 Lua | 📅 2026-06-08 - A plugin for adding/changing/deleting surrounding delimiter pairs.
* [nvim-treesitter/nvim-treesitter-textobjects](https://github.com/nvim-treesitter/nvim-treesitter-textobjects) ⭐ 2,809 | 🐛 124 | 🌐 Tree-sitter Query | 📅 2026-07-19 - Create your own textobjects using Tree-sitter queries.
* [romus204/tree-sitter-manager.nvim](https://github.com/romus204/tree-sitter-manager.nvim) ⭐ 869 | 🐛 17 | 🌐 Tree-sitter Query | 📅 2026-08-03 - A lightweight Tree-sitter parser manager for Neovim 0.12+.
* [m-demare/hlargs.nvim](https://github.com/m-demare/hlargs.nvim) ⭐ 573 | 🐛 6 | 🌐 Lua | 📅 2026-06-05 - Highlight arguments' definitions and usages, using Tree-sitter.
* [RRethy/nvim-treesitter-textsubjects](https://github.com/RRethy/nvim-treesitter-textsubjects) ⭐ 569 | 🐛 7 | 🌐 Tree-sitter Query | 📅 2025-08-14 - Location and syntax aware text objects which *do what you mean*.
* [MeanderingProgrammer/treesitter-modules.nvim](https://github.com/MeanderingProgrammer/treesitter-modules.nvim) ⭐ 169 | 🐛 0 | 🌐 Lua | 📅 2026-05-12 - Original modules from nvim-treesitter master branch.
* [fei6409/log-highlight.nvim](https://github.com/fei6409/log-highlight.nvim) ⭐ 167 | 🐛 0 | 🌐 Vim Script | 📅 2026-05-06 - Generic log syntax highlighting and log filetype management support.
* [LhKipp/nvim-nu](https://github.com/LhKipp/nvim-nu) ⭐ 160 | 🐛 4 | 🌐 Lua | 📅 2024-12-10 - Basic editor support for the nushell language.
* [calops/hmts.nvim](https://github.com/calops/hmts.nvim) ⭐ 96 | 🐛 16 | 🌐 Lua | 📅 2025-06-11 - Tree-sitter queries for Home Manager Nix files.
* [desdic/agrolens.nvim](https://github.com/desdic/agrolens.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2026-06-15 - Navigate via Tree-sitter nodes using Telescope or FZF.
* [Sang-it/fluoride](https://github.com/Sang-it/fluoride) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2026-04-03 - A structural code editor. View, reorder, rename, and annotate code declarations from a floating window based on Tree-sitter.
* [BibekBhusal0/tree-hierarchy.nvim](https://github.com/BibekBhusal0/tree-hierarchy.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-01-10 - Edit text and nevigate based on Tree-sitter.
* [Hdoc1509/gh-actions.nvim](https://github.com/Hdoc1509/gh-actions.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2025-12-16 - Tree-sitter grammar and LSP query configuration for GitHub Actions.
* [bird-chinese-community/BIRD.nvim](https://github.com/bird-chinese-community/BIRD.nvim) ⭐ 2 | 🐛 0 | 🌐 Vim Script | 📅 2026-07-18 - Syntax highlighting, automatic filetype detection, and filetype-specific editing support for BIRD 2 and BIRD 3 configuration files.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Snippet

* [nvim-mini/mini.nvim#mini.snippets](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-snippets.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to manage and expand snippets. Supports LSP snippet syntax, flexible loaders, fuzzy prefix matching, interactive selection, snippet session with rich visualization, and more.
* [L3MON4D3/LuaSnip](https://github.com/L3MON4D3/LuaSnip) ⭐ 4,413 | 🐛 134 | 🌐 Lua | 📅 2026-05-19 - A snippet engine written in Lua.
* [rafamadriz/friendly-snippets](https://github.com/rafamadriz/friendly-snippets) ⭐ 2,769 | 🐛 74 | 🌐 Lua | 📅 2026-01-23 - Set of preconfigured snippets for different languages.
* [chrisgrieser/nvim-scissors](https://github.com/chrisgrieser/nvim-scissors) ⭐ 582 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Automagical editing and creation of snippets.
* [dcampos/nvim-snippy](https://github.com/dcampos/nvim-snippy) ⭐ 341 | 🐛 8 | 🌐 Lua | 📅 2026-06-26 - Snippet plugin written in Lua with support for [vim-snippets](https://github.com/honza/vim-snippets) ⭐ 4,885 | 🐛 83 | 🌐 Vim Snippet | 📅 2025-10-28.
* [ellisonleao/carbon-now.nvim](https://github.com/ellisonleao/carbon-now.nvim) ⭐ 195 | 🐛 1 | 🌐 Lua | 📅 2025-11-05 - Create beautiful code snippets from the terminal.
* [smjonas/snippet-converter.nvim](https://github.com/smjonas/snippet-converter.nvim) ⭐ 183 | 🐛 8 | 🌐 Lua | 📅 2023-09-21 - Convert snippets between the most common snippet formats and modify them using a few lines of Lua code.
* [cvigilv/esqueleto.nvim](https://github.com/cvigilv/esqueleto.nvim) ⭐ 111 | 🐛 5 | 🌐 Lua | 📅 2025-07-09 - Simple templates to use when creating new files.
* [TobinPalmer/rayso.nvim](https://github.com/TobinPalmer/rayso.nvim) ⭐ 86 | 🐛 0 | 🌐 Lua | 📅 2025-11-15 - Create code snippets using [ray.so](https://ray.so).
* [mrcjkb/haskell-snippets.nvim](https://github.com/mrcjkb/haskell-snippets.nvim) ⭐ 35 | 🐛 5 | 🌐 Lua | 📅 2026-06-22 - Haskell snippets for LuaSnip, powered by Tree-sitter and LSP.
* [guilherme-puida/tesoura.nvim](https://github.com/guilherme-puida/tesoura.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2024-06-04 - A flexible snippet system using the native snippet API.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Register

* [acksld/nvim-neoclip.lua](https://github.com/AckslD/nvim-neoclip.lua) ⭐ 1,136 | 🐛 28 | 🌐 Lua | 📅 2025-02-09 - Clipboard manager with telescope integration.
* [gennaro-tedesco/nvim-peekup](https://github.com/gennaro-tedesco/nvim-peekup) ⭐ 338 | 🐛 1 | 🌐 Lua | 📅 2023-02-23 - Dynamically interact with Vim registers.
* [bfredl/nvim-miniyank](https://github.com/bfredl/nvim-miniyank) ⭐ 240 | 🐛 12 | 🌐 Lua | 📅 2023-11-06 - The killring-alike plugin with no default mappings.
* [tenxsoydev/karen-yank.nvim](https://github.com/tenxsoydev/karen-yank.nvim) ⭐ 94 | 🐛 1 | 🌐 Lua | 📅 2023-07-29 - More intentional register handling with delete, cut and yank mappings.
* [kr40/nvim-macros](https://github.com/kr40/nvim-macros) ⭐ 74 | 🐛 1 | 🌐 Lua | 📅 2024-02-16 - Easy way to save and load Macros, with backup and formatting options.
* [desdic/macrothis.nvim](https://github.com/desdic/macrothis.nvim) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2025-02-12 - Save and load macros/registers.
* [tversteeg/registers.nvim](https://codeberg.org/fosk/registers.nvim) - Non-obtrusive minimal preview of Vim registers.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Marks

* [ThePrimeagen/harpoon](https://github.com/ThePrimeagen/harpoon/tree/harpoon2) ⭐ 9,194 | 🐛 146 | 🌐 Lua | 📅 2025-10-31 - A per project, auto updating and editable marks utility for fast file navigation.
* [chentoast/marks.nvim](https://github.com/chentoast/marks.nvim) ⭐ 1,183 | 🐛 56 | 🌐 Lua | 📅 2025-05-13 - A better user experience for viewing and interacting with Vim marks.
* [otavioschwanck/arrow.nvim](https://github.com/otavioschwanck/arrow.nvim) ⭐ 750 | 🐛 34 | 🌐 Lua | 📅 2025-11-28 - Like harpoon, but with a different UX, single keybinding needed and statusline support.
* [cbochs/grapple.nvim](https://github.com/cbochs/grapple.nvim) ⭐ 716 | 🐛 28 | 🌐 Lua | 📅 2024-09-29 - Provides tagging, cursor tracking, and immediate navigation to important project files.
* [LintaoAmons/bookmarks.nvim](https://github.com/LintaoAmons/bookmarks.nvim) ⭐ 294 | 🐛 17 | 🌐 Lua | 📅 2026-07-10 - Your new bookmarks option: simple yet powerful.
* [LeonHeidelbach/trailblazer.nvim](https://github.com/LeonHeidelbach/trailblazer.nvim) ⭐ 284 | 🐛 4 | 🌐 Lua | 📅 2025-02-04 - TrailBlazer introduces a stack based mark system that enables a completely new dynamic and super fast workflow using project wide marks.
* [tomasky/bookmarks.nvim](https://github.com/tomasky/bookmarks.nvim) ⭐ 183 | 🐛 12 | 🌐 Lua | 📅 2024-06-18 - Bookmarks with global file storage, written in Lua.
* [EvWilson/spelunk.nvim](https://github.com/EvWilson/spelunk.nvim) ⭐ 150 | 🐛 0 | 🌐 Lua | 📅 2026-02-27 - Create and manage bookmarks as stacks with a friendly UI.
* [fnune/recall.nvim](https://github.com/fnune/recall.nvim) ⭐ 93 | 🐛 2 | 🌐 Lua | 📅 2026-04-24 - Recall refines the use of marks by focusing on global marks, streamlining their usage and enhancing their visibility and navigability.
* [ofirgall/open.nvim](https://github.com/ofirgall/open.nvim) ⭐ 72 | 🐛 1 | 🌐 Lua | 📅 2026-06-01 - Open the current word with custom openers, GitHub shorthand for example.
* [tristone13th/lspmark.nvim](https://github.com/tristone13th/lspmark.nvim) ⭐ 62 | 🐛 3 | 🌐 Lua | 📅 2026-06-08 - Sane project-wise bookmarks with persistent storage based on LSP.
* [2KAbhishek/markit.nvim](https://github.com/2KAbhishek/markit.nvim) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2025-10-09 - Improved global marks and project wide bookmarks, to quickly navigate files.
* [dimtion/guttermarks.nvim](https://github.com/dimtion/guttermarks.nvim) ⭐ 55 | 🐛 2 | 🌐 Lua | 📅 2026-04-25 - Display marks in the buffer gutter.
* [walkersumida/fusen.nvim](https://github.com/walkersumida/fusen.nvim) ⭐ 43 | 🐛 0 | 🌐 Lua | 📅 2026-07-22 - Sticky note bookmarks, per Git branch with hover annotations and Telescope integration.
* [desdic/marlin.nvim](https://github.com/desdic/marlin.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2026-04-26 - Like harpoon, but with key differences like project path, split support, no UI.
* [heilgar/bookmarks.nvim](https://github.com/heilgar/bookmarks.nvim) ⭐ 28 | 🐛 3 | 🌐 Lua | 📅 2026-05-18 - Manage line bookmarks with Telescope integration and SQLite storage.
* [niuiic/track.nvim](https://github.com/niuiic/track.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2024-11-18 - Enhanced mark with description. Track the thought process of reading source code.
* [zongben/navimark.nvim](https://github.com/zongben/navimark.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-09-17 - An easy and powerful bookmark manager with telescope.
* [y3owk1n/warp.nvim](https://github.com/y3owk1n/warp.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - Simple harpoon alternative that focuses on marking and navigating between files.
* [mohseenrm/marko.nvim](https://github.com/mohseenrm/marko.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-12-01 - Behind the scenes, global marks management for different projects.
* [markgandolfo/dartboard.nvim](https://github.com/markgandolfo/dartboard.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2025-06-08 - Mark files and quickly access them, inspired by Harpoon and Lasso.
* [Beargruug/skipper.nvim](https://github.com/Beargruug/skipper.nvim/) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-07-07 - Jump between functions in a file with ease.
* [adithyasource/spearmint.nvim](https://github.com/adithyasource/spearmint.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-04-29 - Lightweight harpoon-style marks with terminal support.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Search

* [nvim-pack/nvim-spectre](https://github.com/nvim-pack/nvim-spectre) ⭐ 2,406 | 🐛 15 | 🌐 Lua | 📅 2025-05-19 - Search and replace panel.
* [MagicDuck/grug-far.nvim](https://github.com/MagicDuck/grug-far.nvim) ⭐ 1,997 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - Buffer-based live search and replace with full power of `rg` flags. Grug like.
* [kevinhwang91/nvim-hlslens](https://github.com/kevinhwang91/nvim-hlslens) ⭐ 916 | 🐛 11 | 🌐 Lua | 📅 2026-01-11 - Helps you better glance searched information, seamlessly jump matched instances.
* [AckslD/muren.nvim](https://github.com/AckslD/muren.nvim/) ⭐ 366 | 🐛 13 | 🌐 Lua | 📅 2025-02-09 - Multiple replacements through interactive UI.
* [chrisgrieser/nvim-rip-substitute](https://github.com/chrisgrieser/nvim-rip-substitute) ⭐ 319 | 🐛 1 | 🌐 Lua | 📅 2026-08-12 - Search and replace in the current buffer or workspace with incremental preview, a convenient UI, and modern regex syntax.
* [ray-x/sad.nvim](https://github.com/ray-x/sad.nvim) ⭐ 208 | 🐛 4 | 🌐 Lua | 📅 2025-05-01 - Space Age seD integration. Batch file edit tool, a wrapper for [sad](https://github.com/ms-jpq/sad) ⭐ 2,044 | 🐛 28 | 🌐 Rust | 📅 2026-05-11.
* [FabianWirth/search.nvim](https://github.com/FabianWirth/search.nvim) ⭐ 189 | 🐛 7 | 🌐 Lua | 📅 2024-05-21 - Tabs for different Telescope pickers.
* [prochri/telescope-all-recent.nvim](https://github.com/prochri/telescope-all-recent.nvim) ⭐ 149 | 🐛 1 | 🌐 Lua | 📅 2026-06-22 - Frequency and recency sorter for any Telescope picker.
* [2KAbhishek/seeker.nvim](https://github.com/2KAbhishek/seeker.nvim) ⭐ 137 | 🐛 2 | 🌐 Lua | 📅 2026-03-12 - Progressive file seeker built on top of `snacks.nvim`.
* [mangelozzi/rgflow.nvim](https://github.com/mangelozzi/rgflow.nvim) ⭐ 107 | 🐛 1 | 🌐 Lua | 📅 2025-08-11 - Quickly get RipGrep results into an editable Quickfix list, while learning RipGrep's CLI.
* [rktjmp/highlight-current-n.nvim](https://github.com/rktjmp/highlight-current-n.nvim) ⭐ 90 | 🐛 0 | 🌐 Fennel | 📅 2023-06-26 - Highlights the current /, ? or \* match under your cursor when pressing n or N and gets out of the way afterwards.
* [nvimdev/hlsearch.nvim](https://github.com/nvimdev/hlsearch.nvim) ⭐ 83 | 🐛 0 | 🌐 Lua | 📅 2024-01-10 - Auto remove search highlight and rehighlight when using n or N.
* [wurli/visimatch.nvim](https://github.com/wurli/visimatch.nvim) ⭐ 79 | 🐛 5 | 🌐 Lua | 📅 2025-09-25 - Adds highlights to any text matching the current selection in visual mode.
* [polirritmico/telescope-lazy-plugins.nvim](https://github.com/polirritmico/telescope-lazy-plugins.nvim) ⭐ 75 | 🐛 1 | 🌐 Lua | 📅 2025-02-15 - A Telescope picker to quickly access plugins configurations from the lazy.nvim spec.
* [s1n7ax/nvim-search-and-replace](https://github.com/s1n7ax/nvim-search-and-replace) ⭐ 70 | 🐛 1 | 🌐 Lua | 📅 2022-09-06 - Search and replace in multiple files at the same time from the current working directory.
* [backdround/improved-search.nvim](https://github.com/backdround/improved-search.nvim) ⭐ 61 | 🐛 0 | 🌐 Lua | 📅 2023-12-21 - Add search abilities.
* [ankushbhagats/match.nvim](https://github.com/ankushbhagats/match.nvim) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2026-05-06 - Minimal floating search-and-replace with live match tracking, navigation, and quick replacements.
* [duane9/nvim-rg](https://github.com/duane9/nvim-rg) ⭐ 45 | 🐛 0 | 🌐 Vim Script | 📅 2026-08-14 - Run RipGrep asynchronously and see results in a quickfix window.
* [KieranCanter/candela.nvim](https://github.com/KieranCanter/candela.nvim) ⭐ 43 | 🐛 1 | 🌐 Lua | 📅 2026-06-16 - Analyze logs by defining regex patterns to highlight and/or isolate matching lines.
* [wsdjeg/flygrep.nvim](https://github.com/wsdjeg/flygrep.nvim) ⭐ 19 | 🐛 1 | 🌐 Lua | 📅 2026-07-21 - Search text in a floating window asynchronously.
* [bravoecho/brook.nvim](https://github.com/bravoecho/brook.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-07-25 - Responsive, shell-safe ripgrep search for the quickfix list, with native n/N navigation.
* [mahyarmirrashed/search-and-replace.nvim](https://github.com/mahyarmirrashed/search-and-replace.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2025-07-04 - Simple, effective, search and replace functionality for the pragmatic engineer.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Fuzzy Finder

* [nvim-telescope/telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) ⭐ 19,710 | 🐛 459 | 🌐 Lua | 📅 2026-06-27 - Telescope.nvim is a highly [extendable](https://github.com/nvim-telescope/telescope.nvim/wiki/Extensions) ⭐ 19,710 | 🐛 459 | 🌐 Lua | 📅 2026-06-27 A highly extensible fuzzy finder over lists.
* [dmtrKovalenko/fff.nvim](https://github.com/dmtrKovalenko/fff.nvim) ⭐ 10,019 | 🐛 70 | 🌐 Rust | 📅 2026-08-16 - Fuzzy file picker with a standalone native implementation of file indexing and typo resistant fuzzy matcher. Includes all the QOL features, file previews (and images), frecency sorting, last query matching, proximity, Git status bonuses and much more.
* [nvim-mini/mini.nvim#mini.fuzzy](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-fuzzy.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with functions to perform fuzzy matching of one string to others along with fast Telescope sorter.
* [nvim-mini/mini.nvim#mini.pick](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-pick.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with general purpose interactive non-blocking picker that has one window design, toggleable preview, flexible and fast default match, and much more.
* [nvim-mini/mini.nvim#mini.extra](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-extra.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with extra functionality for its modules. Contains 20+ 'mini.pick' pickers, 'mini.ai' textobjects, and more.
* [folke/snacks.nvim#picker](https://github.com/folke/snacks.nvim/blob/main/docs/picker.md) ⭐ 7,971 | 🐛 130 | 🌐 Lua | 📅 2026-05-25 - A modern fuzzy-finder to navigate your editor.
* [ibhagwan/fzf-lua](https://github.com/ibhagwan/fzf-lua) ⭐ 4,419 | 🐛 11 | 🌐 Lua | 📅 2026-08-13 - The Lua version of `fzf.vim`, high-performance and fully async, supports `nvim-web-devicons`, Git indicators, LSP, quickfix/location lists and more. Also supports [`skim`](https://github.com/lotabout/skim) ⭐ 6,924 | 🐛 5 | 🌐 Rust | 📅 2026-08-16 as its fzf binary.
* [nvim-telescope/telescope-media-files.nvim](https://github.com/nvim-telescope/telescope-media-files.nvim) ⭐ 521 | 🐛 36 | 🌐 Lua | 📅 2024-03-30 - Preview images, pdf, epub, video, and fonts using Telescope.
* [camspiers/snap](https://github.com/camspiers/snap) ⭐ 508 | 🐛 28 | 🌐 Fennel | 📅 2026-04-09 - An extensible fuzzy finder. Similar to Telescope, and optimized for performance, especially when grepping in large codebases.
* [bassamsdata/namu.nvim](https://github.com/bassamsdata/namu.nvim) ⭐ 430 | 🐛 7 | 🌐 Lua | 📅 2026-02-17 - Flexible and sleek fuzzy picker, LSP symbol navigator, and more.
* [axkirillov/easypick.nvim](https://github.com/axkirillov/easypick.nvim) ⭐ 410 | 🐛 4 | 🌐 Lua | 📅 2026-08-06 - Easypick lets you easily create Telescope pickers from arbitrary console commands.
* [jvgrootveld/telescope-zoxide](https://github.com/jvgrootveld/telescope-zoxide) ⭐ 370 | 🐛 8 | 🌐 Lua | 📅 2024-08-28 - Telescope integration for [zoxide](https://github.com/ajeetdsouza/zoxide) ⭐ 38,671 | 🐛 136 | 🌐 Rust | 📅 2026-08-10, a smart directory picker that tracks your usage.
* [vijaymarupudi/nvim-fzf](https://github.com/vijaymarupudi/nvim-fzf) ⭐ 348 | 🐛 3 | 🌐 Lua | 📅 2024-10-21 - A Lua API for using FZF. Allows for full asynchronicity for UI speed and usability.
* [linrongbin16/fzfx.nvim](https://github.com/linrongbin16/fzfx.nvim) ⚠️ Archived - A fuzzy finder that updates on every keystroke.
* [fdschmidt93/telescope-egrepify.nvim](https://github.com/fdschmidt93/telescope-egrepify.nvim) ⭐ 144 | 🐛 11 | 🌐 Lua | 📅 2025-12-21 - Telescope plugin for better `rg` flags in `live_grep`.
* [crispgm/telescope-heading.nvim](https://github.com/crispgm/telescope-heading.nvim) ⭐ 142 | 🐛 5 | 🌐 Lua | 📅 2026-03-31 - Telescope extension to switch between headings of AsciiDoc, Markdown, Vimdoc, etc.
* [dtormoen/neural-open.nvim](https://github.com/dtormoen/neural-open.nvim) ⭐ 67 | 🐛 4 | 🌐 Lua | 📅 2026-06-24 - Intelligent `snacks.nvim` picker that teaches a neural network to rank files by what you're most likely to open next.
* [juniorsundar/refer.nvim](https://github.com/juniorsundar/refer.nvim) ⭐ 57 | 🐛 2 | 🌐 Lua | 📅 2026-08-12 - A minimalist picker that doesn't get in your way.
* [wsdjeg/picker.nvim](https://github.com/wsdjeg/picker.nvim) ⭐ 44 | 🐛 1 | 🌐 Lua | 📅 2026-07-24 - Simple fuzzy finder, including files, ctags outline, and more.
* [willyelm/pulse.nvim](https://github.com/willyelm/pulse.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - A single entrypoint for commands. Use prefixes to quickly access diagnostics, Git and more via pickers.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## File Explorer

* [nvim-mini/mini.nvim#mini.files](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-files.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` providing file explorer with column view capable of manipulating file system by editing text. Can create/delete/rename/copy/move files/directories inside and across directories.
* [nvim-tree/nvim-tree.lua](https://github.com/nvim-tree/nvim-tree.lua) ⭐ 8,622 | 🐛 100 | 🌐 Lua | 📅 2026-08-12 - A simple and fast file explorer tree.
* [stevearc/oil.nvim](https://github.com/stevearc/oil.nvim) ⭐ 6,829 | 🐛 148 | 🌐 Lua | 📅 2026-06-02 - Edit your filesystem like a buffer.
* [nvim-neo-tree/neo-tree.nvim](https://github.com/nvim-neo-tree/neo-tree.nvim) ⭐ 5,570 | 🐛 171 | 🌐 Lua | 📅 2026-08-14 - Browse the file system and other tree-like structures in whatever style suits you, including sidebars, floating windows, `netrw` split style, or all of them at once.
* [mikavilpas/yazi.nvim](https://github.com/mikavilpas/yazi.nvim) ⭐ 1,846 | 🐛 12 | 🌐 Lua | 📅 2026-08-15 - Integration with the Yazi terminal file manager.
* [ms-jpq/chadtree](https://github.com/ms-jpq/chadtree) ⭐ 1,690 | 🐛 93 | 🌐 Python | 📅 2026-08-16 - File manager. Better than NERDTree.
* [kevinhwang91/rnvimr](https://github.com/kevinhwang91/rnvimr) ⭐ 845 | 🐛 10 | 🌐 Python | 📅 2026-01-11 - A simple yet amazing file explorer.
* [A7Lavinraj/fyler.nvim](https://github.com/A7Lavinraj/fyler.nvim) ⭐ 761 | 🐛 22 | 🌐 Lua | 📅 2026-08-09 - File manager which can edit file system like a buffer with tree view.
* [luukvbaal/nnn.nvim](https://github.com/luukvbaal/nnn.nvim) ⭐ 464 | 🐛 1 | 🌐 Lua | 📅 2025-04-18 - File explorer powered by [nnn](https://github.com/jarun/nnn) ⭐ 21,794 | 🐛 4 | 🌐 C | 📅 2026-08-16 and Lua.
* [tamago324/lir.nvim](https://github.com/tamago324/lir.nvim) ⭐ 380 | 🐛 10 | 🌐 Lua | 📅 2026-03-29 - Simple file explorer.
* [prichrd/netrw.nvim](https://github.com/prichrd/netrw.nvim) ⭐ 274 | 🐛 4 | 🌐 Lua | 📅 2026-05-05 - Add icons and custom keybindings to netrw.
* [simonmclean/triptych.nvim](https://github.com/simonmclean/triptych.nvim) ⭐ 256 | 🐛 2 | 🌐 Lua | 📅 2026-04-14 - A directory browser inspired by Ranger.
* [X3eRo0/dired.nvim](https://github.com/X3eRo0/dired.nvim) ⭐ 206 | 🐛 4 | 🌐 Lua | 📅 2026-03-05 - A file browser inspired by Emacs Dired.
* [SidOfc/carbon.nvim](https://github.com/SidOfc/carbon.nvim) ⭐ 190 | 🐛 1 | 🌐 Lua | 📅 2026-07-27 - The simple directory tree viewer written in Lua.
* [kelly-lin/ranger.nvim](https://github.com/kelly-lin/ranger.nvim) ⭐ 183 | 🐛 11 | 🌐 Lua | 📅 2024-11-18 - [Ranger](https://github.com/ranger/ranger) ⭐ 17,340 | 🐛 897 | 🌐 Python | 📅 2026-08-15 integration.
* [rolv-apneseth/tfm.nvim](https://github.com/Rolv-Apneseth/tfm.nvim) ⭐ 100 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - Similar to `fm-nvim`, this provides integration for several popular terminal file managers (including [yazi](https://github.com/sxyazi/yazi) ⭐ 41,379 | 🐛 66 | 🌐 Rust | 📅 2026-08-16).
* [Xuyuanp/yanil](https://github.com/Xuyuanp/yanil) ⭐ 99 | 🐛 5 | 🌐 Lua | 📅 2026-01-15 - Yet Another Nerdtree In Lua.
* [theblob42/drex.nvim](https://github.com/TheBlob42/drex.nvim) ⭐ 96 | 🐛 1 | 🌐 Lua | 📅 2025-05-09 - A simple and configurable file explorer written in Lua.
* [ingur/fzf-oil.nvim](https://github.com/ingur/fzf-oil.nvim) ⭐ 68 | 🐛 0 | 🌐 Lua | 📅 2026-07-17 - A tiny file browser with seamless toggling between fzf-lua and oil.nvim.
* [kiran94/s3edit.nvim](https://github.com/kiran94/s3edit.nvim) ⭐ 49 | 🐛 0 | 🌐 Lua | 📅 2025-04-13 - Edit files from Amazon S3.
* [saifulapm/neotree-file-nesting-config](https://github.com/saifulapm/neotree-file-nesting-config) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2025-03-06 - Pre-defined file nesting rules for `neo-tree.nvim`.
* [vodchella/hodur.nvim](https://github.com/vodchella/hodur.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2026-07-06 - Allows you to quickly open a file or copy URL located under cursor.
* [Enigama/miss.nvim](https://github.com/Enigama/miss.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2025-08-17 - Simple popup with changed `unsaved` files, allowing you to save and open them. Helps to avoid forgetting to add something to GitHub or similar.
* [adriancmiranda/glimpse.nvim](https://github.com/adriancmiranda/glimpse.nvim) ⭐ 9 | 🐛 10 | 🌐 Lua | 📅 2026-08-03 - Fast multi-format file previewer with inline kitty graphics support, external pane previews, and integrations for file explorers and pickers.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Project

* [nvim-mini/mini.nvim#mini.visits](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-visits.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to persistently track and reuse file system visits. Allows listing "recent"/"frequent"/"frecent" visits, adding/removing labels to visits and other data.
* [natecraddock/workspaces.nvim](https://github.com/natecraddock/workspaces.nvim) ⭐ 371 | 🐛 8 | 🌐 Lua | 📅 2024-10-08 - Manage workspace directories.
* [GnikDroy/projections.nvim](https://github.com/GnikDroy/projections.nvim) ⭐ 244 | 🐛 8 | 🌐 Lua | 📅 2024-02-05 - Tiny project + session manager.
* [cljoly/telescope-repo.nvim](https://github.com/cljoly/telescope-repo.nvim) ⭐ 241 | 🐛 15 | 🌐 Lua | 📅 2026-05-25 - Telescope picker to jump to any repository (Git or other) on the file system.
* [DrKJeff16/project.nvim](https://github.com/DrKJeff16/project.nvim) ⭐ 197 | 🐛 2 | 🌐 Lua | 📅 2026-08-12 - Project manager with project root detection, documented code and lots of improvements, including `snacks.nvim`, `fzf-lua` and `picker.nvim` support.
* [klen/nvim-config-local](https://github.com/klen/nvim-config-local) ⭐ 180 | 🐛 5 | 🌐 Lua | 📅 2025-01-21 - Secure load local config files from working directories.
* [LintaoAmons/cd-project.nvim](https://github.com/LintaoAmons/cd-project.nvim) ⭐ 133 | 🐛 6 | 🌐 Lua | 📅 2026-08-12 - All you need is just an easier way to `cd` to another project directory.
* [windwp/nvim-projectconfig](https://github.com/windwp/nvim-projectconfig) ⭐ 112 | 🐛 5 | 🌐 Lua | 📅 2024-07-28 - Load specific configs depending on the project directory.
* [otavioschwanck/telescope-alternate.nvim](https://github.com/otavioschwanck/telescope-alternate.nvim) ⭐ 107 | 🐛 5 | 🌐 Lua | 📅 2025-07-05 - Alternate between common files using telescope.
* [OscarCreator/rsync.nvim](https://github.com/OscarCreator/rsync.nvim) ⭐ 102 | 🐛 8 | 🌐 Lua | 📅 2024-08-08 - Automatically sync up/down project to a remote with rsync.
* [mrjones2014/codesettings.nvim](https://github.com/mrjones2014/codesettings.nvim) ⭐ 84 | 🐛 5 | 🌐 Lua | 📅 2026-08-15 - Easily load project-local settings (like `.vscode/settings.json`) into native LSP settings.
* [SalOrak/whaler.nvim](https://github.com/SalOrak/whaler.nvim) ⭐ 75 | 🐛 0 | 🌐 Lua | 📅 2026-06-22 - Telescope extension to move between directories blazingly fast.
* [nyngwang/suave.lua](https://github.com/nyngwang/suave.lua) ⭐ 69 | 🐛 10 | 🌐 Lua | 📅 2025-08-02 - Multi-tabs project session automation.
* [Abstract-IDE/penvim](https://github.com/Abstract-IDE/penvim) ⭐ 51 | 🐛 1 | 🌐 Lua | 📅 2022-07-23 - Project's root directory and documents Indentation detector with project based config loader.
* [karnull/switchboard.nvim](https://github.com/karnull/switchboard.nvim) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - Define "run", "build", or any custom command/bind per language or project, then use the same keybinds everywhere.
* [desdic/telescope-rooter.nvim](https://github.com/desdic/telescope-rooter.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2024-05-18 - Makes sure to always start telescope (and only telescope) from the project/root directory.
* [wsdjeg/rooter.nvim](https://github.com/wsdjeg/rooter.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2026-08-16 - Change working directory to project root.
* [josephschmitt/pj.nvim](https://github.com/josephschmitt/pj.nvim) ⭐ 23 | 🐛 1 | 🌐 Lua | 📅 2026-04-03 - Automatic project discovery with configurable depth with multiple pickers supported (Snacks, Telescope, fzf-lua).
* [zachyarbrough/anchor.nvim](https://github.com/zachyarbrough/anchor.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-08-05 - Pin project-specific directories for instant fuzzy searching. Inspired by Harpoon.
* [zongben/proot.nvim](https://github.com/zongben/proot.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-04-10 - Lightweight project navigator with telescope.
* [martuscellifaria/ahoicpp.nvim](https://github.com/martuscellifaria/ahoicpp.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-08-14 - Sets up C++ projects on a modular fashion and helps newcomers with the language heavy lifting.
* [Rimkomatic/vimtagger.nvim](https://github.com/Rimkomatic/vimtagger.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-06-27 - Semantic file tagging for projects with Telescope integration. Organize files using custom tags, search them quickly, and manage tags through an interactive UI.
* [LucasTavaresA/headers.nvim](https://github.com/LucasTavaresA/headers.nvim) ⭐ 5 | 🐛 1 | 🌐 Lua | 📅 2026-06-11 - Zero-config header/footer warnings.
* [cosmicbuffalo/root\_swapper.nvim](https://github.com/cosmicbuffalo/root_swapper.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-08 - Lightweight root swapper that uses `lcd` to swap to the appropriate root directory based on the current buffer.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Buffers

* [famiu/bufdelete.nvim](https://github.com/famiu/bufdelete.nvim) ⚠️ Archived - Delete buffers without losing your window layout.
* [rgroli/other.nvim](https://github.com/rgroli/other.nvim) ⭐ 491 | 🐛 9 | 🌐 Lua | 📅 2025-05-09 - Open alternative files for the current buffer.
* [j-morano/buffer\_manager.nvim](https://github.com/j-morano/buffer_manager.nvim) ⭐ 399 | 🐛 5 | 🌐 Lua | 📅 2026-02-04 - Add one or more buffers, reorder them, save them inside a file or just delete them very easily from a small floating window.
* [chrisgrieser/nvim-early-retirement](https://github.com/chrisgrieser/nvim-early-retirement) ⭐ 256 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Send buffers into early retirement by automatically closing them after x minutes of inactivity.
* [axkirillov/hbac.nvim](https://github.com/axkirillov/hbac.nvim) ⭐ 222 | 🐛 0 | 🌐 Lua | 📅 2026-05-04 - Automatically close buffers you are not working on.
* [kazhala/close-buffers.nvim](https://github.com/kazhala/close-buffers.nvim) ⭐ 173 | 🐛 6 | 🌐 Lua | 📅 2023-06-02 - Delete multiple Vim buffers based on different conditions.
* [dzfrias/arena.nvim](https://github.com/dzfrias/arena.nvim) ⭐ 118 | 🐛 3 | 🌐 Lua | 📅 2026-03-15 - A smart (frecency-based) buffer switcher.
* [m-demare/attempt.nvim](https://github.com/m-demare/attempt.nvim) ⭐ 94 | 🐛 0 | 🌐 Lua | 📅 2026-06-05 - Manage and run temporary buffers.
* [ahkohd/buffer-sticks.nvim](https://github.com/ahkohd/buffer-sticks.nvim) ⭐ 85 | 🐛 1 | 🌐 Lua | 📅 2026-07-29 - Cosmetic buffers indicator and picker.
* [backdround/tabscope.nvim](https://github.com/backdround/tabscope.nvim) ⭐ 59 | 🐛 5 | 🌐 Lua | 📅 2023-10-09 - Make tab-local buffers.
* [francescarpi/buffon.nvim](https://github.com/francescarpi/buffon.nvim) ⭐ 34 | 🐛 4 | 🌐 Lua | 📅 2026-06-26 - Buffers navigation, reorganize and close.
* [sQVe/bufignore.nvim](https://github.com/sQVe/bufignore.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-01-08 - Unlist hidden buffers matching specified ignore sources.
* [wsdjeg/bufdel.nvim](https://github.com/wsdjeg/bufdel.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2026-07-16 - Delete buffers without changing windows layout.
* [ChuufMaster/buffer-vacuum](https://github.com/ChuufMaster/buffer-vacuum) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2025-08-18 - Set a maximum number of buffers to keep open and intelligently delete the oldest buffers over the maximum.
* [TheLazyCat00/workspaces-nvim](https://github.com/TheLazyCat00/workspaces-nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-06-05 - Pin files to specific keys within a project workspace, giving you quick access to your most important files.
* [akasataikisiti/tabLocalBuffer.nvim](https://github.com/akasataikisiti/tabLocalBuffer.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-05-16 - Keeps a per-tab buffer list and provides its own bnext / bprevious style navigation that cycles only within the current tab.
* [mong8se/buffish.nvim](https://github.com/mong8se/buffish.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-10-13 - A buffer switcher in the spirit of dirvish or vinegar.
* [BibekBhusal0/bufstack.nvim](https://github.com/BibekBhusal0/bufstack.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-06-26 - Track recently visited buffers and reopen recently closed buffers.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Color

* [nvim-mini/mini.nvim#mini.hipatterns](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-hipatterns.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to highlight patterns in text with configurable highlighters. Works asynchronously with configurable debounce delay.
* [folke/twilight.nvim](https://github.com/folke/twilight.nvim) ⭐ 1,544 | 🐛 3 | 🌐 Lua | 📅 2025-10-28 - Dim inactive portions of the code you're editing using Tree-sitter.
* [catgoose/nvim-colorizer.lua](https://github.com/catgoose/nvim-colorizer.lua) ⭐ 1,117 | 🐛 5 | 🌐 Lua | 📅 2026-07-14 - A high-performance color highlighter which has no external dependencies.
* [uga-rosa/ccc.nvim](https://github.com/uga-rosa/ccc.nvim) ⭐ 978 | 🐛 12 | 🌐 Lua | 📅 2025-05-06 - Super powerful color picker / colorizer plugin.
* [TaDaa/vimade](https://github.com/TaDaa/vimade) ⭐ 675 | 🐛 8 | 🌐 Lua | 📅 2026-07-16 - Dim, fade, tint, animate, and customize colors in your windows and buffers.
* [nvzone/minty](https://github.com/nvzone/minty) ⭐ 604 | 🐛 2 | 🌐 Lua | 📅 2025-02-28 - Beautifully crafted color tools.
* [xzbdmw/colorful-menu.nvim](https://github.com/xzbdmw/colorful-menu.nvim) ⭐ 497 | 🐛 8 | 🌐 Lua | 📅 2026-06-30 - Colorize your auto completion menu using Tree-sitter.
* [max397574/colortils.nvim](https://github.com/max397574/colortils.nvim) ⭐ 431 | 🐛 8 | 🌐 Lua | 📅 2025-01-10 - Provides utils to work with colors (picker, conversion).
* [rasulomaroff/reactive.nvim](https://github.com/rasulomaroff/reactive.nvim) ⭐ 248 | 🐛 9 | 🌐 Lua | 📅 2025-12-30 - Set global and window-specific highlights or trigger callbacks when modes/operators change or windows are switched.
* [winston0410/range-highlight.nvim](https://github.com/winston0410/range-highlight.nvim) ⭐ 216 | 🐛 3 | 🌐 Lua | 📅 2025-12-10 - An extremely lightweight plugin (\~ 120loc) that highlights ranges you have entered in commandline.
* [miversen33/sunglasses.nvim](https://github.com/miversen33/sunglasses.nvim) ⭐ 160 | 🐛 7 | 🌐 Lua | 📅 2025-01-13 - Dynamic Colorscheme/highlight adjuster on window switching.
* [rachartier/tiny-devicons-auto-colors.nvim](https://github.com/rachartier/tiny-devicons-auto-colors.nvim) ⭐ 134 | 🐛 0 | 🌐 Lua | 📅 2026-05-29 - Automatically updates nvim-web-devicons colors based on your current colorscheme.
* [Mr-LLLLL/interestingwords.nvim](https://github.com/Mr-LLLLL/interestingwords.nvim) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2024-08-19 - Highlight multiple word same time and navigate word under cursor with scrolling smoothly, display search count in virualtext.
* [lcheylus/overlength.nvim](https://github.com/lcheylus/overlength.nvim) ⭐ 52 | 🐛 0 | 🌐 Lua | 📅 2026-04-07 - A small plugin to highlight too long lines.
* [leolaurindo/tunnelvision.nvim](https://github.com/leolaurindo/tunnelvision.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2026-07-30 - Focus on one symbol at a time by dimming unrelated lines.
* [moyiz/command-and-cursor.nvim](https://github.com/moyiz/command-and-cursor.nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2025-03-30 - Highlight cursor and visual selections when entering command mode.
* [wsdjeg/cpicker.nvim](https://github.com/wsdjeg/cpicker.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-07-21 - A lightweight color palette plugin that supports a wide range of color models.
* [3ZsForInsomnia/pacer.nvim](https://github.com/3ZsForInsomnia/pacer.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-03-17 - Creates a reading pacer by highlighting one word at a time and dimming all text outside the current paragraph-and-some to help you read faster.
* [cxwx/shadowMyName.nvim](https://github.com/cxwx/shadowMyName.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-06-24 - Redact sensitive words such as your username, tokens, phone numbers and more when recording your screen.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Colorscheme

Each colorscheme will have one or more of the tags listed below. If a tag is missing
then it is not supported:

<!--lint disable awesome-list-item-->

* ***`[TS]`*** - Has Tree-sitter highlighting.
* ***`[LSP]`*** - Has LSP Semantic Tokens support.
* ***`[L/D]`*** - Has both "light" and "dark" variants.
* ***`[Lua]`*** - Is written in Lua.
* ***`[Fnl]`*** - Is written in Fennel.

<!--lint enable awesome-list-item-->

* [folke/tokyonight.nvim](https://github.com/folke/tokyonight.nvim) ⭐ 8,169 | 🐛 20 | 🌐 Lua | 📅 2026-03-24 - ***`[TS][LSP][L/D][Lua]`*** A clean, dark and light theme written in Lua, with support for LSP, Tree-sitter and lots of plugins.
* [sainnhe/everforest](https://github.com/sainnhe/everforest) ⭐ 4,173 | 🐛 6 | 🌐 Vim Script | 📅 2026-06-08 - ***`[TS][LSP][L/D]`*** A green based colorscheme designed to be warm, soft and easy on the eyes.
* [sainnhe/gruvbox-material](https://github.com/sainnhe/gruvbox-material) ⭐ 2,628 | 🐛 8 | 🌐 Vim Script | 📅 2026-04-15 - ***`[TS][LSP]`*** Gruvbox modification with softer contrast and Tree-sitter support.
* [projekt0n/github-nvim-theme](https://github.com/projekt0n/github-nvim-theme) ⭐ 2,473 | 🐛 28 | 🌐 Lua | 📅 2024-12-31 - ***`[TS][LSP][L/D][Lua]`*** A GitHub theme, kitty, alacritty written in Lua. Support built-in LSP and Tree-sitter.
* [navarasu/onedark.nvim](https://github.com/navarasu/onedark.nvim) ⭐ 2,003 | 🐛 57 | 🌐 Lua | 📅 2026-04-13 - ***`[TS][LSP][Lua]`*** A One Dark Theme written in Lua based on Atom's One Dark Theme.
* [sainnhe/sonokai](https://github.com/sainnhe/sonokai) ⭐ 1,954 | 🐛 1 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP]`*** High Contrast and Vivid Color Scheme based on Monokai Pro.
* [nyoom-engineering/oxocarbon.nvim](https://github.com/nyoom-engineering/oxocarbon.nvim) ⭐ 1,622 | 🐛 21 | 🌐 Fennel | 📅 2026-08-09 - ***`[TS][LSP][L/D][Lua]`*** A dark and light theme written in Fennel, inspired by IBM Carbon.
* [dracula/vim](https://github.com/dracula/vim) ⭐ 1,390 | 🐛 8 | 🌐 Vim Script | 📅 2026-08-09 - ***`[TS][LSP]`*** Famous beautiful dark powered theme.
* [bluz71/vim-moonfly-colors](https://github.com/bluz71/vim-moonfly-colors) ⭐ 1,319 | 🐛 0 | 🌐 Lua | 📅 2026-05-30 - ***`[TS][LSP][Lua]`*** A dark charcoal colorscheme with Tree-sitter support.
* [mhartington/oceanic-next](https://github.com/mhartington/oceanic-next) ⭐ 1,179 | 🐛 10 | 🌐 Vim Script | 📅 2025-10-10 - ***`[TS][L/D]`*** Oceanic Next theme.
* [marko-cerovac/material.nvim](https://github.com/marko-cerovac/material.nvim) ⭐ 1,089 | 🐛 6 | 🌐 Lua | 📅 2026-02-23 - ***`[TS][LSP][L/D][Lua]`*** Material.nvim is a highly configurable colorscheme written in Lua and based on the material palette.
* [AlexvZyl/nordic.nvim](https://github.com/AlexvZyl/nordic.nvim) ⭐ 1,052 | 🐛 3 | 🌐 Lua | 📅 2026-05-03 - ***`[TS][Lua]`*** Nord theme, but warmer and darker. Supports a variety of plugins and other platforms.
* [sainnhe/edge](https://github.com/sainnhe/edge) ⭐ 1,040 | 🐛 2 | 🌐 Vim Script | 📅 2026-01-21 - ***`[TS][LSP][L/D]`*** Clean and Elegant Color Scheme inspired by Atom One and Material.
* [shaunsingh/nord.nvim](https://github.com/shaunsingh/nord.nvim) ⭐ 1,016 | 🐛 33 | 🌐 Lua | 📅 2024-06-25 - ***`[TS][Lua]`*** A colorscheme based off of the Nord Color Palette.
* [tomasiser/vim-code-dark](https://github.com/tomasiser/vim-code-dark) ⭐ 1,000 | 🐛 15 | 🌐 Vim Script | 📅 2024-05-21 - ***`[TS]`*** A dark color scheme heavily inspired by the look of the Dark+ scheme of VSCode.
* [Mofiqul/vscode.nvim](https://github.com/Mofiqul/vscode.nvim) ⭐ 991 | 🐛 50 | 🌐 Lua | 📅 2025-12-03 - ***`[TS][L/D][Lua]`*** A Lua port of vim-code-dark colorscheme with VSCode light and dark theme.
* [savq/melange-nvim](https://github.com/savq/melange-nvim) ⭐ 973 | 🐛 12 | 🌐 Lua | 📅 2025-12-10 - ***`[TS][LSP][L/D][Lua]`*** Warm colorscheme written in Lua with support for various terminal emulators.
* [bluz71/vim-nightfly-colors](https://github.com/bluz71/vim-nightfly-colors) ⭐ 942 | 🐛 0 | 🌐 Lua | 📅 2026-05-30 - ***`[TS][LSP][Lua]`*** A dark midnight colorscheme with Tree-sitter support.
* [fenetikm/falcon](https://github.com/fenetikm/falcon) ⭐ 845 | 🐛 12 | 🌐 Vim Script | 📅 2026-07-02 - ***`[TS][Lua]`*** A colour scheme for terminals, Vim and friends.
* [Mofiqul/dracula.nvim](https://github.com/Mofiqul/dracula.nvim) ⭐ 779 | 🐛 24 | 🌐 Lua | 📅 2025-11-05 - ***`[TS]`*** Dracula colorscheme written in Lua.
* [everviolet/nvim](https://github.com/everviolet/nvim) ⭐ 677 | 🐛 0 | 🌐 Lua | 📅 2026-07-22 - ***`[TS][LSP][L/D][Lua]`*** A comfy colorscheme for cozy morning coding.
* [neanias/everforest-nvim](https://github.com/neanias/everforest-nvim) ⭐ 456 | 🐛 8 | 🌐 Lua | 📅 2026-07-27 - ***`[TS][LSP][L/D][Lua]`*** A Lua port of the Everforest colour scheme.
* [tanvirtin/monokai.nvim](https://github.com/tanvirtin/monokai.nvim) ⭐ 392 | 🐛 14 | 🌐 Lua | 📅 2023-12-02 - ***`[TS][LSP][Lua]`*** Monokai theme written in Lua.
* [nvimdev/zephyr-nvim](https://github.com/nvimdev/zephyr-nvim) ⭐ 377 | 🐛 3 | 🌐 Lua | 📅 2022-12-31 - ***`[TS][Lua]`*** A dark colorscheme with Tree-sitter support.
* [ray-x/aurora](https://github.com/ray-x/aurora) ⭐ 377 | 🐛 1 | 🌐 Lua | 📅 2026-05-09 - ***`[TS][LSP][Lua]`*** A 24-bit dark theme with Tree-sitter and LSP support.
* [oskarnurm/koda.nvim](https://github.com/oskarnurm/koda.nvim) ⭐ 343 | 🐛 2 | 🌐 Lua | 📅 2026-06-11 - ***`[TS][LSP][L/D][Lua]`*** Code's quiet companion. A minimalist colorscheme, written in Lua.
* [ChristianChiarulli/nvcode-color-schemes.vim](https://github.com/ChristianChiarulli/nvcode-color-schemes.vim) ⭐ 304 | 🐛 21 | 🌐 Vim script | 📅 2024-07-08 - ***`[TS]`*** Nvcode, onedark, nord colorschemes with Tree-sitter support.
* [rockerBOO/boo-colorscheme-nvim](https://github.com/rockerBOO/boo-colorscheme-nvim) ⭐ 288 | 🐛 3 | 🌐 Lua | 📅 2026-07-06 - ***`[TS][Lua]`*** A colorscheme with handcrafted support for LSP, Tree-sitter.
* [NTBBloodbath/doom-one.nvim](https://github.com/NTBBloodbath/doom-one.nvim) ⭐ 250 | 🐛 10 | 🌐 Lua | 📅 2025-06-28 - ***`[TS][L/D][Lua]`*** Lua port of doom-emacs' doom-one.
* [datsfilipe/vesper.nvim](https://github.com/datsfilipe/vesper.nvim) ⭐ 248 | 🐛 1 | 🌐 Lua | 📅 2025-04-21 - ***`[TS][LSP][Lua]`*** It's a port of the popular VS Code theme Vesper, written in Lua.
* [ray-x/starry.nvim](https://github.com/ray-x/starry.nvim) ⭐ 246 | 🐛 3 | 🌐 Lua | 📅 2026-04-09 - ***`[TS][LSP][L/D][Lua]`*** A collection of modern colorschemes: `material`, `moonlight`, `dracula (blood)`, `monokai`, `mariana`, `emerald`, `earlysummer`, `middlenight_blue`, `darksolar`.
* [askfiy/visual\_studio\_code](https://github.com/askfiy/visual_studio_code) ⭐ 212 | 🐛 4 | 🌐 Lua | 📅 2024-09-24 - ***`[TS][LSP][L/D][Lua]`***  A theme that highly restores VSCode.
* [rafamadriz/neon](https://github.com/rafamadriz/neon) ⭐ 209 | 🐛 2 | 🌐 Lua | 📅 2022-11-27 - ***`[TS][LSP][L/D][Lua]`*** Customizable colorscheme with excellent italic and bold support, dark and light variants. Made to work and look good with Tree-sitter.
* [Tsuzat/NeoSolarized.nvim](https://github.com/Tsuzat/NeoSolarized.nvim) ⚠️ Archived - ***`[TS][LSP][L/D][Lua]`*** NeoSolarized colorscheme with full transparency.
* [ishan9299/nvim-solarized-lua](https://github.com/ishan9299/nvim-solarized-lua) ⭐ 209 | 🐛 16 | 🌐 Lua | 📅 2024-03-04 - ***`[TS][Lua]`*** Solarized colorscheme written in Lua.
* [ThorstenRhau/token](https://github.com/ThorstenRhau/token) ⭐ 182 | 🐛 0 | 🌐 Lua | 📅 2026-08-09 - ***`[TS][LSP][L/D][Lua]`*** Token has warm tones and careful contrast, with full Tree-sitter and LSP integration.
* [ishan9299/modus-theme-vim](https://github.com/ishan9299/modus-theme-vim) ⭐ 178 | 🐛 4 | 🌐 Lua | 📅 2022-10-09 - ***`[TS][L/D][Lua]`*** This is a color scheme developed by Protesilaos Stavrou for emacs.
* [kdheepak/monochrome.nvim](https://github.com/kdheepak/monochrome.nvim) ⭐ 177 | 🐛 1 | 🌐 Lua | 📅 2021-07-14 - ***`[TS][Lua]`*** A 16-bit monochrome colorscheme that uses [HSLuv](https://www.hsluv.org/) for perceptually distinct gray colors, with support for Tree-sitter and other commonly used plugins.
* [andersevenrud/nordic.nvim](https://github.com/andersevenrud/nordic.nvim) ⭐ 174 | 🐛 4 | 🌐 Lua | 📅 2024-06-16 - ***`[TS][Lua]`*** A nord-esque colorscheme.
* [svrana/neosolarized.nvim](https://github.com/svrana/neosolarized.nvim) ⭐ 166 | 🐛 6 | 🌐 Lua | 📅 2025-06-12 - ***`[TS][LSP][Lua]`*** Dark solarized colorscheme using colorbuddy for easy customization.
* [serhez/teide.nvim](https://github.com/serhez/teide.nvim) ⭐ 165 | 🐛 2 | 🌐 Lua | 📅 2026-01-12 - ***`[TS][LSP][L/D][Lua]`*** A fork of folke's `tokyonight.nvim` with a different color palette.
* [niyabits/calvera-dark.nvim](https://github.com/niyabits/calvera-dark.nvim) ⭐ 161 | 🐛 4 | 🌐 Lua | 📅 2021-12-23 - ***`[TS][Lua]`*** A port of the [VSCode Calvara Dark](https://github.com/saurabhdaware/vscode-calvera-dark) ⭐ 12 | 🐛 1 | 🌐 HTML | 📅 2024-08-17 theme with support for Tree-sitter and many other plugins.
* [uhs-robert/oasis.nvim](https://github.com/uhs-robert/oasis.nvim) ⭐ 151 | 🐛 1 | 🌐 CSS | 📅 2026-08-15 - ***`[TS][LSP][L/D][Lua]`*** Desert theme ported from Vim and made modern with 12 variants, a collection of dark themes for every color of the rainbow.
* [ofirgall/ofirkai.nvim](https://github.com/ofirgall/ofirkai.nvim) ⭐ 139 | 🐛 15 | 🌐 Lua | 📅 2026-08-05 - ***`[TS][LSP][Lua]`*** Monokai theme that aims to feel like Sublime Text.
* [Th3Whit3Wolf/one-nvim](https://github.com/Th3Whit3Wolf/one-nvim) ⭐ 120 | 🐛 5 | 🌐 Lua | 📅 2021-07-26 - ***`[TS][L/D][Lua]`*** An Atom One inspired dark and light colorscheme.
* [Abstract-IDE/Abstract-cs](https://github.com/Abstract-IDE/Abstract-cs) ⭐ 119 | 🐛 2 | 🌐 Lua | 📅 2025-10-27 - ***`[TS][LSP][Lua]`*** Colorscheme written in Lua, specially made for roshnivim with Tree-sitter support.
* [Th3Whit3Wolf/onebuddy](https://github.com/Th3Whit3Wolf/onebuddy) ⭐ 100 | 🐛 4 | 🌐 Lua | 📅 2021-04-01 - ***`[TS][L/D][Lua]`*** Light and dark atom one theme.
* [sontungexpt/witch](https://github.com/sontungexpt/witch) ⭐ 79 | 🐛 2 | 🌐 Lua | 📅 2025-11-25 - ***`[TS][LSP][L/D][Lua]`*** The primary stinvim distro colorscheme includes the default feature of dimming inactive windows, along with various other customization options for users.
* [datsfilipe/min-theme.nvim](https://github.com/datsfilipe/min-theme.nvim) ⭐ 61 | 🐛 1 | 🌐 Lua | 📅 2024-08-03 - ***`[TS][LSP][Lua]`*** It's a port of Min, a minimal theme for VSCode, written in Lua.
* [Th3Whit3Wolf/space-nvim](https://github.com/Th3Whit3Wolf/space-nvim) ⭐ 51 | 🐛 2 | 🌐 Lua | 📅 2024-05-28 - ***`[TS][L/D][Lua]`*** A spacemacs inspired dark and light colorscheme.
* [bkegley/gloombuddy](https://github.com/bkegley/gloombuddy) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2021-04-16 - ***`[TS][Lua]`*** Gloom inspired theme.
* [adisen99/codeschool.nvim](https://github.com/adisen99/codeschool.nvim) ⭐ 45 | 🐛 0 | 🌐 Lua | 📅 2026-02-10 - ***`[TS][LSP][Lua]`*** Codeschool colorscheme written in Lua with Tree-sitter and built-in LSP support.
* [nxvu699134/vn-night.nvim](https://github.com/nxvu699134/vn-night.nvim) ⭐ 44 | 🐛 0 | 🌐 Lua | 📅 2025-02-17 - ***`[Lua]`*** A dark colorscheme written in Lua.
* [yonatan-perel/lake-dweller.nvim](https://github.com/yonatan-perel/lake-dweller.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2026-05-18 - ***`[TS][LSP][Lua]`*** Dark and opinionated with selective highlighting aiming to be readable at a glance.
* [github-main-user/lytmode.nvim](https://github.com/github-main-user/lytmode.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2026-07-05 - ***`[TS][LSP][Lua]`*** A unique in-between theme inspired by LYT-Mode for Obsidian. Not quite dark, not quite light — just right.
* [silentium-theme/silentium.nvim](https://github.com/silentium-theme/silentium.nvim) ⭐ 31 | 🐛 1 | 🌐 Lua | 📅 2026-08-05 - ***`[TS][Luа]`*** Pragmatic and monochrome theme with the goal to increase reading speed and reduce eye strain by highlighting only what is needed.
* [wurli/cobalt.nvim](https://github.com/wurli/cobalt.nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - ***`[TS][LSP][Lua]`*** A (mostly) faithful port of the classic blue theme from TextMate.
* [jim-at-jibba/ariake.nvim](https://github.com/jim-at-jibba/ariake.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-11-11 - ***`[TS][LSP][Lua]`*** A port of the great Atom theme. Beautiful, dark colour scheme.
* [kuri-sun/yoda.nvim](https://github.com/kuri-sun/yoda.nvim) ⚠️ Archived - ***`[TS][L/D][Lua]`*** Muted green palette for focused, balanced editing.
* [jthvai/lavender.nvim](https://codeberg.org/jthvai/lavender.nvim) - ***`[TS][LSP][Lua]`*** Purple-hued dark mode colorscheme; a complete rewrite of shaunsingh/moonlight.nvim.

<!--lint disable awesome-spell-check-->

* [rose-pine/neovim](https://github.com/rose-pine/neovim) ⭐ 3,070 | 🐛 5 | 🌐 Lua | 📅 2026-05-15 - ***`[TS][LSP][L/D][Lua]`*** All natural pine, faux fur and a bit of soho vibes for the classy minimalist.

<!--lint enable awesome-spell-check-->

* [nvim-mini/mini.nvim#colorschemes](https://github.com/nvim-mini/mini.nvim#plugin-color-schemes) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - ***`[TS][LSP][L/D][Lua]`*** Color schemes included in `mini.nvim`. All of them prioritize high contrast ratio for reading text and computing palettes in perceptually uniform color spaces.
* [catppuccin/nvim](https://github.com/catppuccin/nvim) ⭐ 7,572 | 🐛 11 | 🌐 Lua | 📅 2026-08-09 - ***`[TS][LSP][L/D][Lua]`*** Warm mid-tone dark theme to show off your vibrant self! With support for native LSP, Tree-sitter, and more.
* [rebelot/kanagawa.nvim](https://github.com/rebelot/kanagawa.nvim) ⭐ 6,336 | 🐛 90 | 🌐 Lua | 📅 2026-05-10 - ***`[TS][LSP][L/D][Lua]`*** A dark colorscheme inspired by the colors of the famous painting by Katsushika Hokusai.
* [EdenEast/nightfox.nvim](https://github.com/EdenEast/nightfox.nvim) ⭐ 4,063 | 🐛 37 | 🌐 Lua | 📅 2026-07-04 - ***`[TS][LSP][L/D][Lua]`*** A soft dark, fully customizable colorscheme with support for LSP, Tree-sitter and a variety of plugins.
* [ellisonleao/gruvbox.nvim](https://github.com/ellisonleao/gruvbox.nvim) ⭐ 2,596 | 🐛 28 | 🌐 Lua | 📅 2026-04-15 - ***`[TS][LSP][L/D][Lua]`*** Gruvbox community colorscheme Lua port.
* [scottmckendry/cyberdream.nvim](https://github.com/scottmckendry/cyberdream.nvim) ⭐ 1,386 | 🐛 1 | 🌐 Lua | 📅 2026-08-15 - ***`[TS][L/D][Lua]`*** A high-contrast, futuristic and vibrant coloursheme.
* [zenbones-theme/zenbones.nvim](https://github.com/zenbones-theme/zenbones.nvim) ⭐ 1,137 | 🐛 21 | 🌐 Vim Script | 📅 2026-06-26 - ***`[TS][LSP][L/D][Lua]`*** A collection of colorschemes designed to highlight code using contrasts and font variations.
* [olimorris/onedarkpro.nvim](https://github.com/olimorris/onedarkpro.nvim) ⭐ 1,090 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - ***`[TS][L/D][Lua]`*** Atom's iconic One Dark theme. Cacheable, fully customisable, Tree-sitter and LSP semantic token support. Comes with light and dark variants.
* [embark-theme/vim](https://github.com/embark-theme/vim) ⭐ 733 | 🐛 1 | 🌐 Vim Script | 📅 2026-07-21 - ***`[TS]`*** A deep inky purple theme leveraging bright colors.
* [rmehri01/onenord.nvim](https://github.com/rmehri01/onenord.nvim) ⭐ 640 | 🐛 0 | 🌐 Lua | 📅 2026-07-01 - ***`[TS][LSP][L/D][Lua]`*** A colorscheme that combines the Nord and Atom One Dark color palettes for a more vibrant programming experience.
* [slugbyte/lackluster.nvim](https://github.com/slugbyte/lackluster.nvim) ⭐ 576 | 🐛 0 | 🌐 Lua | 📅 2025-10-06 - ***`[TS][LSP][Lua]`*** A delightful mostly grayscale colorscheme that is soft on the eyes, and supports heaps of plugins.
* [xero/miasma.nvim](https://github.com/xero/miasma.nvim) ⭐ 565 | 🐛 6 | 🌐 Vim Script | 📅 2025-07-12 - ***`[TS][LSP]`*** A dark pastel color scheme inspired by the woods. Built using lush and supports Tree-sitter, diagnostics, CMP, Git-Signs, Telescope, Which-key, Lazy, and more.
* [ribru17/bamboo.nvim](https://github.com/ribru17/bamboo.nvim) ⭐ 485 | 🐛 5 | 🌐 Lua | 📅 2025-11-25 - ***`[TS][LSP][Lua]`*** A warm green theme.
* [luisiacc/gruvbox-baby](https://github.com/luisiacc/gruvbox-baby) ⭐ 460 | 🐛 7 | 🌐 Lua | 📅 2024-01-25 - ***`[TS][LSP][Lua]`*** A modern gruvbox theme with full Tree-sitter support.
* [uloco/bluloco.nvim](https://github.com/uloco/bluloco.nvim) ⭐ 451 | 🐛 10 | 🌐 Lua | 📅 2026-04-21 - ***`[TS][LSP][L/D][Lua]`*** A fancy and sophisticated colorscheme for night and day coding. Supports LSP, Tree-sitter and all the plugins you love.
* [ramojus/mellifluous.nvim](https://github.com/ramojus/mellifluous.nvim) ⭐ 449 | 🐛 3 | 🌐 Lua | 📅 2026-04-20 - ***`[TS][LSP][L/D][Lua]`*** Pleasant and productive colorscheme.
* [miikanissi/modus-themes.nvim](https://github.com/miikanissi/modus-themes.nvim) ⭐ 446 | 🐛 3 | 🌐 Lua | 📅 2026-08-12 - ***`[TS][LSP][L/D][Lua]`*** Accessible theme, conforming with the highest standard for color contrast (WCAG AAA).
* [mellow-theme/mellow.nvim](https://github.com/mellow-theme/mellow.nvim) ⭐ 430 | 🐛 2 | 🌐 Lua | 📅 2026-03-30 - ***`[TS][LSP][Lua]`*** A soothing dark color scheme with Tree-sitter support.
* [thesimonho/kanagawa-paper.nvim](https://github.com/thesimonho/kanagawa-paper.nvim) ⭐ 398 | 🐛 2 | 🌐 Lua | 📅 2026-05-26 - ***`[TS][LSP][L/D][Lua]`*** Remixed light and dark Kanagawa colourschemes with muted colors.
* [oxfist/night-owl.nvim](https://github.com/oxfist/night-owl.nvim) ⭐ 352 | 🐛 5 | 🌐 Lua | 📅 2024-09-12 - ***`[TS][LSP][Lua]`*** A [Night Owl colorscheme port from VSCode](https://github.com/sdras/night-owl-vscode-theme) ⭐ 2,957 | 🐛 48 | 📅 2024-12-31 with support for Tree-sitter and semantic tokens.
* [FrenzyExists/aquarium-vim](https://github.com/FrenzyExists/aquarium-vim) ⭐ 325 | 🐛 5 | 🌐 Vim Script | 📅 2026-06-28 - ***`[TS][L/D]`*** A dark, yet vibrant colorscheme.
* [gbprod/nord.nvim](https://github.com/gbprod/nord.nvim) ⭐ 311 | 🐛 7 | 🌐 Lua | 📅 2026-04-14 - ***`[TS][LSP][Lua]`*** An arctic, north-bluish clean and elegant theme, based on Nord Palette.
* [maxmx03/fluoromachine.nvim](https://github.com/maxmx03/fluoromachine.nvim) ⭐ 310 | 🐛 1 | 🌐 Lua | 📅 2025-10-21 - ***`[TS][LSP][Lua]`*** Synthwave x Fluoromachine port.
* [Everblush/nvim](https://github.com/Everblush/nvim) ⭐ 302 | 🐛 4 | 🌐 Lua | 📅 2025-05-18 - ***`[TS][LSP][Lua]`*** A dark, vibrant and beautiful colorscheme written in Lua.
* [Mofiqul/adwaita.nvim](https://github.com/Mofiqul/adwaita.nvim) ⭐ 295 | 🐛 13 | 🌐 Lua | 📅 2026-06-02 - ***`[TS][LSP][L/D][Lua]`*** Colorscheme based on GNOME Adwaita syntax with support for popular plugins.
* [0xstepit/flow.nvim](https://github.com/0xstepit/flow.nvim) ⭐ 285 | 🐛 4 | 🌐 Lua | 📅 2026-05-21 - ***`[TS][L/D][Lua]`*** Carefully designed colors to help focusing during coding plus fluorescent details. Support many plugins and tools.
* [zootedb0t/citruszest.nvim](https://github.com/zootedb0t/citruszest.nvim) ⭐ 266 | 🐛 2 | 🌐 Lua | 📅 2026-04-16 - ***`[TS][LSP][Lua]`*** A colorscheme that features a combination of bright and juicy colors reminiscent of various citrus fruits, with LSP and Tree-sitter support.
* [dasupradyumna/midnight.nvim](https://github.com/dasupradyumna/midnight.nvim) ⭐ 236 | 🐛 2 | 🌐 Lua | 📅 2024-11-01 - ***`[TS][LSP][Lua]`*** A modern black theme with comfortable color contrast for a pleasant visual experience, with LSP and Tree-sitter support.
* [diegoulloao/neofusion.nvim](https://github.com/diegoulloao/neofusion.nvim) ⭐ 234 | 🐛 0 | 🌐 Lua | 📅 2026-03-02 - ***`[TS][LSP][Lua]`*** A theme compatible with Tree-sitter inspired by `gruvbox.nvim`.
* [rockyzhang24/arctic.nvim](https://github.com/rockyzhang24/arctic.nvim) ⭐ 219 | 🐛 2 | 🌐 Lua | 📅 2024-12-18 - ***`[TS][LSP][Lua]`*** A colorscheme ported from VSCode Dark+ theme with the strict and precise color picking for both the editor and UI.
* [cpea2506/one\_monokai.nvim](https://github.com/cpea2506/one_monokai.nvim) ⭐ 192 | 🐛 1 | 🌐 Lua | 📅 2026-06-21 - ***`[TS][LSP][Lua]`*** One Monokai theme written in Lua.
* [Verf/deepwhite.nvim](https://github.com/Verf/deepwhite.nvim) ⭐ 181 | 🐛 0 | 🌐 Lua | 📅 2026-06-11 - ***`[TS][LSP][Lua]`*** A light colorscheme inspired by [flatwhite-syntax](https://github.com/biletskyy/flatwhite-syntax) ⭐ 198 | 🐛 15 | 🌐 CSS | 📅 2020-04-27 and [elegant-emacs](https://github.com/rougier/elegant-emacs) ⭐ 1,447 | 🐛 8 | 🌐 Emacs Lisp | 📅 2021-11-22.
* [polirritmico/monokai-nightasty.nvim](https://github.com/polirritmico/monokai-nightasty.nvim) ⭐ 167 | 🐛 0 | 🌐 Lua | 📅 2026-07-16 - ***`[TS][LSP][L/D][Lua]`*** A dark/light theme based on the Monokai color palette written in Lua, support for LSP, Tree-sitter and lots of plugins.
* [HoNamDuong/hybrid.nvim](https://github.com/HoNamDuong/hybrid.nvim) ⭐ 162 | 🐛 0 | 🌐 Lua | 📅 2026-05-03 - ***`[TS][LSP][Lua]`*** A dark theme written in Lua.
* [Aejkatappaja/cendre](https://github.com/Aejkatappaja/cendre) ⭐ 145 | 🐛 1 | 🌐 Lua | 📅 2026-08-12 - ***`[TS][LSP][Lua]`*** Dark colorscheme with every hue computed from a wood fire's emission spectrum, plus matching ports for terminals and tools.
* [nyngwang/nvimgelion](https://github.com/nyngwang/nvimgelion) ⭐ 139 | 🐛 4 | 🌐 Vim Script | 📅 2024-03-07 - ***`[TS]`*** Neon Genesis Evangelion but for Vimmers.
* [jpwol/thorn.nvim](https://github.com/jpwol/thorn.nvim) ⭐ 127 | 🐛 0 | 🌐 Lua | 📅 2026-05-17 - ***`[TS][LSP][L/D][Lua]`*** A rich green theme with dark and light options. Supports LSP, transparency, many plugins, and more.
* [metalelf0/jellybeans-nvim](https://github.com/metalelf0/jellybeans-nvim) ⭐ 127 | 🐛 2 | 🌐 Lua | 📅 2025-01-15 - ***`[TS][Lua]`*** A port of jellybeans colorscheme.
* [lalitmee/cobalt2.nvim](https://github.com/lalitmee/cobalt2.nvim) ⭐ 116 | 🐛 0 | 🌐 Lua | 📅 2025-10-30 - ***`[Lua]`*** A port of cobalt2 colorscheme using colorbuddy.
* [phha/zenburn.nvim](https://github.com/phha/zenburn.nvim) ⭐ 112 | 🐛 3 | 🌐 Lua | 📅 2024-07-02 - ***`[TS][Lua]`*** A low-contrast dark colorscheme with support for various plugins.
* [ptdewey/darkearth-nvim](https://github.com/ptdewey/darkearth-nvim) ⭐ 89 | 🐛 0 | 🌐 Fennel | 📅 2026-06-03 - ***`[TS][LSP][Fnl]`*** A dark and earthy colorscheme supporting Tree-sitter and LSP.
* [killitar/obscure.nvim](https://github.com/killitar/obscure.nvim) ⭐ 81 | 🐛 4 | 🌐 Lua | 📅 2026-01-27 - ***`[TS][LSP][Lua]`*** A pastel dark colorscheme inspired by the palette Mellow. Support Tree-sitter, LSP *(including semantic tokens)* and lots of plugins.
* [cryptomilk/nightcity.nvim](https://github.com/cryptomilk/nightcity.nvim) ⭐ 72 | 🐛 0 | 🌐 Lua | 📅 2026-04-24 - ***`[TS][LSP][Lua]`*** A dark colorscheme inspired by Inkpot, Jellybeans, Gruvbox and Tokyonight with LSP support.
* [lewpoly/sherbet.nvim](https://github.com/lewpoly/sherbet.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2022-12-17 - ***`[TS][Lua]`*** A soothing colorscheme with support for popular plugins and Tree-sitter.
* [ldelossa/vimdark](https://github.com/ldelossa/vimdark) ⭐ 69 | 🐛 0 | 🌐 Vim script | 📅 2022-03-20 - ***`[TS][L/D]`*** A minimal Vim theme for night time. Loosely based on vim-monotonic and chrome's dark reader extension. A light theme is included as well for the day time.
* [2nthony/vitesse.nvim](https://github.com/2nthony/vitesse.nvim) ⭐ 68 | 🐛 1 | 🌐 Lua | 📅 2024-08-17 - ***`[TS][LSP][Lua]`*** Vitesse theme Lua port.
* [samharju/synthweave.nvim](https://github.com/samharju/synthweave.nvim) ⭐ 67 | 🐛 1 | 🌐 Lua | 📅 2025-09-25 - ***`[TS][LSP][Lua]`*** Synthwave '84 colorscheme port.
* [Aejkatappaja/sora](https://github.com/Aejkatappaja/sora) ⭐ 67 | 🐛 1 | 🌐 Lua | 📅 2026-08-10 - ***`[TS][LSP][Lua]`*** Deep blue-black dark colorscheme with one ethereal cyan accent, with matching ports for many terminal apps and tools.
* [mitander/flume.nvim](https://github.com/mitander/flume.nvim) ⭐ 61 | 🐛 0 | 🌐 Lua | 📅 2026-07-27 - ***`[TS][LSP][L/D][Lua]`*** Four-palette color system with consistent semantic roles and matching generated themes for terminal and developer tools.
* [hyperb1iss/silkcircuit](https://github.com/hyperb1iss/silkcircuit) ⭐ 55 | 🐛 2 | 🌐 Lua | 📅 2026-07-26 - ***`[TS][LSP][L/D][Lua]`*** Vibrant cyberpunk color system with five variants, 40+ plugin integrations, WCAG AA compliant. Supports multiple editors, terminals and CLI tools.
* [samharju/serene.nvim](https://github.com/samharju/serene.nvim) ⭐ 51 | 🐛 0 | 🌐 Lua | 📅 2024-08-08 - ***`[TS][Lua]`*** A soothing and dark Tree-sitter/LSP-supported theme for relaxing your eyes after using more vibrant colorschemes.
* [adisen99/apprentice.nvim](https://github.com/adisen99/apprentice.nvim) ⭐ 50 | 🐛 0 | 🌐 Lua | 📅 2026-02-20 - ***`[TS][L/D][Lua]`*** Colorscheme written in Lua based on the [Apprentice](https://github.com/romainl/Apprentice) ⭐ 930 | 🐛 1 | 🌐 Vim Script | 📅 2025-07-14 color palette with Tree-sitter and built-in LSP support.
* [uncleTen276/dark\_flat.nvim](https://github.com/uncleTen276/dark_flat.nvim) ⭐ 43 | 🐛 3 | 🌐 Lua | 📅 2024-06-19 - ***`[TS][LSP][Lua]`*** A colorscheme written in Lua ported from Dark Flat iTerm2 theme, with LSP and Tree-sitter support.
* [ankushbhagats/pastel.nvim](https://github.com/ankushbhagats/pastel.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2026-04-18 - ***`[TS][LSP][L/D][Lua]`*** Elegant pastel colorschemes with advanced customization, styles, and integrations.
* [marekh19/meowsoot.nvim](https://github.com/marekh19/meowsoot.nvim) ⭐ 34 | 🐛 2 | 🌐 Lua | 📅 2026-07-19 - ***`[TS][LSP][L/D][Lua]`*** A dark pink–cyan–lavender colorscheme where strings are yellow and green never reaches code.
* [calind/selenized.nvim](https://github.com/calind/selenized.nvim) ⭐ 32 | 🐛 3 | 🌐 Lua | 📅 2025-08-06 - ***`[TS][LSP][L/D][Lua]`*** Lua port of [selenized](https://github.com/jan-warchol/selenized) ⭐ 929 | 🐛 58 | 🌐 Emacs Lisp | 📅 2025-09-28 with support for Tree-sitter, `nvim-cmp`, GitSigns, and more.
* [titanzero/zephyrium](https://github.com/titanzero/zephyrium) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2022-02-20 - ***`[TS][Lua]`*** A zephyr-esque theme, written in Lua, with Tree-sitter support.
* [alexmozaidze/palenight.nvim](https://github.com/alexmozaidze/palenight.nvim) ⭐ 27 | 🐛 0 | 🌐 Fennel | 📅 2026-07-27 - ***`[TS][LSP][Fnl]`*** Palenight colorscheme supporting Tree-sitter, LSP *(including semantic tokens)* and lots of plugins.
* [T-b-t-nchos/Aquavium.nvim](https://github.com/T-b-t-nchos/Aquavium.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2026-06-02 - ***`[TS][Lua]`*** Aquarium-themed color scheme, designed for use with a transparent terminal background.
* [qaptoR-nvim/chocolatier.nvim](https://github.com/qaptoR-nvim/chocolatier.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-07-07 - ***`[TS][LSP][Lua]`*** An espresso/kimbie inspired chocolatey theme adapted from ellisonleao/gruvbox.nvim theme as a code template.
* [loganswartz/sunburn.nvim](https://github.com/loganswartz/sunburn.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-03-26 - ***`[TS][Lua]`*** A colorscheme sitting somewhere between pastels and solarized, emphasizing readability and hue uniformity above all else.
* [chrsm/paramount-ng.nvim](https://github.com/chrsm/paramount-ng.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2022-06-18 - ***`[TS][Lua]`*** A dark color scheme written using Lush. Tree-sitter supported.
* [54L1M/Oshen.nvim](https://github.com/54L1M/Oshen.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-06-12 - ***`[TS][LSP][L/D][Lua]`*** Inspired by deep ocean water at night, derived entirely from five source colors.
* [judaew/ronny.nvim](https://github.com/judaew/ronny.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-04-08 - ***`[TS][LSP][Lua]`*** A dark colorscheme, which mostly was inspired by the Monokai originally created by Wimem Hazenberg.
* [bakageddy/alduin.nvim](https://github.com/bakageddy/alduin.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2024-01-27 - ***`[TS][LSP][Lua]`*** A port of [alduin](https://github.com/AlessandroYorba/alduin) ⭐ 486 | 🐛 9 | 🌐 Vim script | 📅 2022-08-31 theme to Lua with Tree-sitter and semantic highlights support.
* [pebeto/dookie.nvim](https://github.com/pebeto/dookie.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-05-05 - ***`[TS][Lua]`*** A color scheme inspired by Plan9's acme editor.
* [dybdeskarphet/gruvbox-minimal.nvim](https://github.com/dybdeskarphet/gruvbox-minimal.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-07-11 - ***`[TS][L/D][Lua]`*** A Gruvbox Material theme conceptually inspired by Alabaster.
* [sonjiku/yawnc.nvim](https://github.com/sonjiku/yawnc.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2023-06-25 - ***`[TS][LSP][Lua]`*** Theming using pywal, with a Base16 twist.
* [pmouraguedes/neodarcula.nvim](https://github.com/pmouraguedes/neodarcula.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-02-01 - ***`[TS][LSP][Lua]`*** A dark theme with support for transparency, dimming, LSP semantic tokens and more.
* [0x-ximon/acario.nvim](https://github.com/0x-ximon/acario.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-07-05 - ***`[TS][LSP][L/D][Lua]`*** A port of the clean, high-contrast Doom Emacs Acario theme.
* [ptdewey/monalisa-nvim](https://github.com/ptdewey/monalisa-nvim) ⭐ 11 | 🐛 0 | 🌐 Fennel | 📅 2025-08-20 - ***`[TS][LSP][Lua]`*** A dark and colorful Mona Lisa inspired colorscheme.
* [y3owk1n/base16-pro-max.nvim](https://github.com/y3owk1n/base16-pro-max.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - ***`[TS][LSP][Lua]`*** Base16 with 16 colors + syntax, transparency, dimmed inactive panes, semantic aliases, live blends, overrides, and first-class plugin integrations.
* [samesense/savitsky.nvim](https://github.com/samesense/savitsky.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-01-18 - ***`[TS][LSP][L/D][Lua]`*** Curated color palettes inspired by paintings from the Savitsky Museum, built on top of `catppuccin`.
* [ntk148v/lauds](https://github.com/ntk148v/lauds) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-07-09 - ***`[TS][Lua]`*** Paper-light color theme for prose and code — warm off-white paper, terracotta orange, deep mint.
* [kevinm6/kurayami.nvim](https://github.com/kevinm6/kurayami.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2025-11-01 - ***`[TS][LSP][Lua]`*** Dark only theme with Tree-sitter support.
* [ntk148v/slack.nvim](https://github.com/ntk148v/slack.nvim) ⭐ 6 | 🐛 1 | 🌐 Lua | 📅 2025-06-12 - ***`[TS][L/D][Lua]`*** A ported Slack colorscheme.
* [taigrr/cyberpunk.nvim](https://github.com/taigrr/cyberpunk.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-08-08 - ***`[TS][LSP][Lua]`*** Dark neon colorscheme with green, cyan, yellow, and red highlights on a black background.
* [alsi-lawr/neotheme.nvim](https://github.com/alsi-lawr/neotheme.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-07-23 - ***`[TS][LSP][L/D][Lua]`*** A semantic, palette-driven theme engine, with live theme switching and multiple built-in families.
* [aadielpr/bono.nvim](https://github.com/aadielpr/bono.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-08-07 - ***`[TS][LSP][Lua]`*** A warm muted colorscheme with cream (light) variants.
* [tan-wei/zimablue.nvim](https://github.com/tan-wei/zimablue.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-07-31 - ***`[TS][LSP][Lua]`*** A dark Neovim colorscheme inspired by the iconic color from the *Love, Death and Robots* episode *Zima Blue*.
* [art220/dancheong.nvim](https://github.com/art220/dancheong.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - ***`[TS][LSP][L/D][Lua]`*** Four variants drawn from dancheong, the 1,500-year-old Korean temple-painting palette, with every color contrast-gated at build time and a matching lualine theme.
* [micdzu/aalto.nvim](https://github.com/micdzu/aalto.nvim) - ***`[TS][LSP][L/D][Lua]`*** A semantic colorscheme with a perceptual OKLCH engine, featuring four semantic roles and both dark and light variants.
* [sxwpb/halfspace.nvim](https://gitlab.com/sxwpb/halfspace.nvim) - ***`[TS][LSP][Lua]`*** A semi-light colorscheme for minimal eye melting.
* [bartekjaszczak/distinct-nvim](https://gitlab.com/bartekjaszczak/distinct-nvim) - ***`[TS][LSP][L/D][Lua]`*** Theme with distinct syntax colours. Supports Tree-sitter and semantic highlighting. For people who love multi-colour syntax highlighting.
* [bartekjaszczak/luma-nvim](https://gitlab.com/bartekjaszczak/luma-nvim) - ***`[TS][LSP][L/D][Lua]`*** A colorful theme with dark/light modes and adjustable contrast. Supports Tree-sitter and semantic highlighting.
* [bartekjaszczak/finale-nvim](https://gitlab.com/bartekjaszczak/finale-nvim) - ***`[TS][LSP][Lua]`*** A balanced dark theme, blending vivid and pastel colors for a comfortable, high-contrast experience. Supports Tree-sitter and semantic highlighting.
* [m15a/nvim-srcerite](https://codeberg.org/m15a/nvim-srcerite) - ***`[TS][Lua]`*** A colorscheme inspired by [Srcery](https://srcery.sh/), based on `nvim-highlite`.
* [motaz-shokry/gruvbox.nvim](https://gitlab.com/motaz-shokry/gruvbox.nvim) - ***`[TS][L/D][Lua]`*** A new gruvbox theme with a different background color for the hard variant, and comes with 4 variants.
* [brargenzilian/darcula-solid.nvim](https://codeberg.org/brargenzilian/darcula-solid.nvim) - ***`[TS][Lua]`*** A color-scheme that was heavily inspired by the JetBrains IntelliJ IDEA default theme, but was carefully refined to bring a more pleasant, aesthetic, and contrasting experience.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

### Colorscheme Creation

* [nvim-mini/mini.nvim#mini.base16](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-base16.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with fast implementation of base16 theme for manually supplied palette.
* [nvim-mini/mini.nvim#mini.colors](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-colors.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to tweak and save any color scheme. Also can animate transition and convert between some color spaces.
* [nvim-mini/mini.nvim#mini.hues](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-hues.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to generate configurable color scheme. Takes only background and foreground colors as required arguments. Can adjust number of hues for non-base colors, saturation, accent color, plugin integration.
* [rktjmp/lush.nvim](https://github.com/rktjmp/lush.nvim) ⭐ 1,782 | 🐛 13 | 🌐 Lua | 📅 2025-09-01 - Define colorschemes as a DSL in Lua, with real-time feedback.
* [tjdevries/colorbuddy.nvim](https://github.com/tjdevries/colorbuddy.nvim) ⭐ 785 | 🐛 4 | 🌐 Lua | 📅 2024-05-08 - A colorscheme helper. Written in Lua! Quick and Easy Color Schemes.
* [RRethy/base16-nvim](https://github.com/RRethy/base16-nvim) ⭐ 649 | 🐛 2 | 🌐 Lua | 📅 2026-08-10 - A base16 colorscheme builder. Includes support for Tree-sitter and LSP highlight groups.
* [svermeulen/text-to-colorscheme](https://github.com/svermeulen/text-to-colorscheme) ⭐ 317 | 🐛 6 | 🌐 Lua | 📅 2024-08-14 - Allows the user to generate colorschemes with a text prompt using OpenAI's GPT API.
* [ThemerCorp/themer.lua](https://github.com/ThemerCorp/themer.lua) ⭐ 262 | 🐛 7 | 🌐 Lua | 📅 2023-10-17 - Create colorschemes for your editor and supported apps (such as `kitty` and `alacritty`).
* [Iron-E/nvim-highlite](https://github.com/Iron-E/nvim-highlite) ⭐ 252 | 🐛 2 | 🌐 Lua | 📅 2026-06-17 - A colorscheme generator that is "lite" on logic for the developer.
* [norcalli/nvim-base16.lua](https://github.com/norcalli/nvim-base16.lua) ⭐ 79 | 🐛 2 | 🌐 Lua | 📅 2023-04-11 - Programmatic Lua library for setting base16 themes.
* [loganswartz/polychrome.nvim](https://github.com/loganswartz/polychrome.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - A colorscheme micro-framework, with support for specifying colors directly in many different formats (sRGB, HSL, Oklab, XYZ and more, with intelligent chroma clipping), live editing preview, and a simple DSL.
* [Senal-D-A-Gunaratna/matugen.nvim](https://github.com/Senal-D-A-Gunaratna/matugen.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - Material You colorscheme generator using an external template system. Supports Tree-sitter, LSP, and Lua.
* [nitinbhat972/cwal.nvim](https://github.com/nitinbhat972/cwal.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-08-15 - Generates dynamic colorschemes from cwal-generated color palettes.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

### Colorscheme Switchers

* [f-person/auto-dark-mode.nvim](https://github.com/f-person/auto-dark-mode.nvim) ⭐ 504 | 🐛 10 | 🌐 Lua | 📅 2026-03-29 - Follow the system appearance on macOS.
* [zaldih/themery.nvim](https://github.com/zaldih/themery.nvim) ⭐ 382 | 🐛 19 | 🌐 Lua | 📅 2025-01-01 - A new way to change the colorscheme on the fly like in VSCode.
* [LmanTW/themify.nvim](https://github.com/LmanTW/themify.nvim/tree/main) ⭐ 63 | 🐛 1 | 🌐 Lua | 📅 2025-05-13 - A lightweight colorscheme manager and switcher inspired by Themery.nvim and Lazy.nvim.
* [CWood-sdf/pineapple](https://github.com/CWood-sdf/pineapple) ⭐ 58 | 🐛 0 | 🌐 Lua | 📅 2026-08-08 - Install any colorscheme in your config without leaving your terminal. Collects every colorscheme on the internet and allows you to preview them all before installing.
* [linrongbin16/colorbox.nvim](https://github.com/linrongbin16/colorbox.nvim) ⭐ 50 | 🐛 1 | 🌐 Lua | 📅 2026-04-13 - Load all the ultra colorschemes into your editor's player.
* [4e554c4c/darkman.nvim](https://github.com/4e554c4c/darkman.nvim) ⭐ 41 | 🐛 3 | 🌐 Go | 📅 2025-04-06 - Follow the system dark-mode setting on Linux.
* [Erl-koenig/theme-hub.nvim](https://github.com/Erl-koenig/theme-hub.nvim) ⭐ 31 | 🐛 0 | 🌐 Lua | 📅 2025-10-19 - Manage and install colorschemes via telescope-pickers.
* [itsfernn/auto-gnome-theme.nvim](https://github.com/itsfernn/auto-gnome-theme.nvim) ⭐ 15 | 🐛 1 | 🌐 Lua | 📅 2025-12-02 - Fast colorscheme switcher following GNOME system's light/dark mode (based on `gsetting monitor`).
* [flashcodes-themayankjha/fkthemes.nvim](https://github.com/flashcodes-themayankjha/fkthemes.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2025-11-14 - A fast, lightweight and powerful theme switcher written in Lua.
* [DrKJeff16/which-colorscheme.nvim](https://github.com/DrKJeff16/which-colorscheme.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-08-06 - Cycle between colorschemes using either custom or autogenerated `which-key.nvim` bindings.
* [nishu-murmu/ThemeSwitch.nvim](https://github.com/nishu-murmu/ThemeSwitch.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-06-26 - Light weight color scheme switcher.
* [BrunoCiccarino/gardenal](https://github.com/BrunoCiccarino/gardenal) - Gardenal is a theme switcher, which allows the user to create keyboard shortcuts to switch between themes with one click.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Bars and Lines

* [SmiteshP/nvim-navic](https://github.com/SmiteshP/nvim-navic) ⭐ 1,679 | 🐛 30 | 🌐 Lua | 📅 2025-12-29 - A simple statusline/winbar component that uses LSP to show your current code context.
* [Bekaboo/dropbar.nvim](https://github.com/Bekaboo/dropbar.nvim) ⭐ 1,591 | 🐛 14 | 🌐 Lua | 📅 2026-05-31 - IDE-like breadcrumbs, out of the box.
* [utilyre/barbecue.nvim](https://github.com/utilyre/barbecue.nvim) ⚠️ Archived - A VSCode like winbar.
* [luukvbaal/statuscol.nvim](https://github.com/luukvbaal/statuscol.nvim) ⭐ 613 | 🐛 9 | 🌐 Lua | 📅 2026-07-09 - Configurable 'statuscolumn' with built-in segments and click handlers.
* [m4xshen/smartcolumn.nvim](https://github.com/m4xshen/smartcolumn.nvim) ⭐ 370 | 🐛 3 | 🌐 Lua | 📅 2026-07-20 - Hide your colorcolumn when unneeded.
* [Bekaboo/deadcolumn.nvim](https://github.com/Bekaboo/deadcolumn.nvim) ⭐ 351 | 🐛 2 | 🌐 Lua | 📅 2025-09-04 - Shows your colorcolumn dynamically.
* [ecthelionvi/NeoColumn.nvim](https://github.com/ecthelionvi/NeoColumn.nvim) ⚠️ Archived - Toggleable colorcolumn highlighting specific characters.
* [OXY2DEV/bars.nvim](https://github.com/OXY2DEV/bars.nvim) ⭐ 95 | 🐛 1 | 🌐 Lua | 📅 2026-05-31 - A starting point/guide for creating custom statusline, statuscolumn, tabline and winbar.
* [mawkler/hml.nvim](https://github.com/mawkler/hml.nvim) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2024-11-21 - Adds `H`/`M`/`L` indicators to your line numbers.
* [zaakiy/line-justice.nvim](https://github.com/zaakiy/line-justice.nvim) ⭐ 16 | 🐛 0 | 🌐 Lua | 📅 2026-05-07 - Shows both absolute and relative line numbers simultaneously.
* [neur1n/noline.nvim](https://github.com/neur1n/noline.nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2025-07-11 - Fully customizable bars and lines components with no presets nor constraints.

### Statusline

* [nvim-mini/mini.nvim#mini.statusline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-statusline.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for minimal and fast statusline. Supports content change depending on window width.
* [nvim-lualine/lualine.nvim](https://github.com/nvim-lualine/lualine.nvim) ⭐ 8,093 | 🐛 270 | 🌐 Lua | 📅 2026-05-31 - Easily configurable, blazingly fast statusline.
* [rebelot/heirline.nvim](https://github.com/rebelot/heirline.nvim) ⭐ 1,286 | 🐛 28 | 🌐 Lua | 📅 2025-05-23 - A no-nonsense statusline designed around recursive inheritance to be exceptionally fast and versatile.
* [b0o/incline.nvim](https://github.com/b0o/incline.nvim) ⭐ 1,046 | 🐛 10 | 🌐 Lua | 📅 2026-05-07 - Lightweight floating statuslines, intended for use with the new global statusline.
* [windwp/windline.nvim](https://github.com/windwp/windline.nvim) ⭐ 532 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - The next generation statusline. Animation statusline.
* [tamton-aquib/staline.nvim](https://github.com/tamton-aquib/staline.nvim) ⭐ 399 | 🐛 8 | 🌐 Lua | 📅 2024-06-02 - A modern lightweight statusline in Lua. Mainly uses unicode symbols for showing info.
* [tjdevries/express\_line.nvim](https://github.com/tjdevries/express_line.nvim) ⭐ 316 | 🐛 20 | 🌐 Lua | 📅 2024-05-17 - Supports co-routines, functions and jobs.
* [adelarsq/neoline.vim](https://github.com/adelarsq/neoline.vim) ⭐ 271 | 🐛 11 | 🌐 Lua | 📅 2026-04-08 - A light statusline/tabline plugin using Lua.
* [beauwilliams/statusline.lua](https://github.com/beauwilliams/statusline.lua) ⭐ 264 | 🐛 5 | 🌐 Lua | 📅 2025-04-30 - A zero-config minimal statusline written in Lua featuring awesome integrations and blazing speed.
* [ojroques/nvim-hardline](https://github.com/ojroques/nvim-hardline) ⭐ 208 | 🐛 2 | 🌐 Lua | 📅 2023-12-27 - A statusline / bufferline inspired by [vim-airline](https://github.com/vim-airline/vim-airline) ⭐ 17,962 | 🐛 37 | 🌐 Vim Script | 📅 2026-07-25 that aims to be as light and simple as possible.
* [MunifTanjim/nougat.nvim](https://github.com/MunifTanjim/nougat.nvim) ⭐ 201 | 🐛 3 | 🌐 Lua | 📅 2024-01-07 - Hyperextensible statusline/tabline/winbar.
* [NTBBloodbath/galaxyline.nvim](https://github.com/NTBBloodbath/galaxyline.nvim) ⭐ 172 | 🐛 13 | 🌐 Lua | 📅 2022-05-16 - A light-weight and super fast statusline plugin written in Lua.
* [Zeioth/heirline-components.nvim](https://github.com/Zeioth/heirline-components.nvim) ⭐ 159 | 🐛 3 | 🌐 Lua | 📅 2026-02-25 - 30+ `heirline.nvim` components to be used out of the box to create the perfect user interface.
* [sschleemilch/slimline.nvim](https://github.com/sschleemilch/slimline.nvim) ⭐ 138 | 🐛 3 | 🌐 Lua | 📅 2026-08-03 - A slim, minimal and opinionated Lua statusline.
* [sontungexpt/witch-line](https://github.com/sontungexpt/witch-line) ⭐ 65 | 🐛 1 | 🌐 Lua | 📅 2026-07-15 - A blazing fast statusline based on reference concept.
* [yaocccc/nvim-lines.lua](https://github.com/yaocccc/nvim-lines.lua) ⭐ 40 | 🐛 0 | 🌐 Lua | 📅 2023-04-06 - A fast, light, customizable statusline and tabline (buffers).
* [tajirhas9/muslim.nvim](https://github.com/tajirhas9/muslim.nvim) ⭐ 37 | 🐛 0 | 🌐 Lua | 📅 2026-03-03 - Get prayer times and useful islamic essentials in your statusline.
* [konapun/vacuumline.nvim](https://github.com/konapun/vacuumline.nvim) ⭐ 30 | 🐛 1 | 🌐 Lua | 📅 2023-02-18 - A galaxyline configuration inspired by airline.
* [mikesmithgh/git-prompt-string-lualine.nvim](https://github.com/mikesmithgh/git-prompt-string-lualine.nvim) ⭐ 27 | 🐛 1 | 🌐 Lua | 📅 2024-04-22 - Add git-prompt-string to your statusline.
* [Mr-LLLLL/lualine-ext.nvim](https://github.com/Mr-LLLLL/lualine-ext.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-10-21 - Show more information on lualine.

### Tabline

* [nvim-mini/mini.nvim#mini.tabline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-tabline.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for minimal tabline showing listed buffers in case of one tab and falling back to default otherwise.
* [akinsho/bufferline.nvim](https://github.com/akinsho/bufferline.nvim) ⭐ 4,364 | 🐛 103 | 🌐 Lua | 📅 2025-01-14 - A snazzy bufferline built using Lua.
* [romgrk/barbar.nvim](https://github.com/romgrk/barbar.nvim) ⭐ 2,723 | 🐛 35 | 🌐 Lua | 📅 2026-06-10 - A tabline with re-orderable, auto-sizing, clickable tabs, icons, nice highlighting, sort-by commands and a magic jump-to-buffer mode.
* [nanozuki/tabby.nvim](https://github.com/nanozuki/tabby.nvim) ⭐ 770 | 🐛 8 | 🌐 Lua | 📅 2026-01-07 - A minimal, configurable tabline that allows using tabs as workspace multiplexers.
* [willothy/nvim-cokeline](https://github.com/willothy/nvim-cokeline) ⭐ 634 | 🐛 13 | 🌐 Lua | 📅 2026-06-19 - A bufferline for people with addictive personalities.
* [alvarosevilla95/luatab.nvim](https://github.com/alvarosevilla95/luatab.nvim) ⭐ 210 | 🐛 8 | 🌐 Lua | 📅 2025-03-21 - A simple tabline written in Lua.
* [rafcamlet/tabline-framework.nvim](https://github.com/rafcamlet/tabline-framework.nvim) ⭐ 102 | 🐛 4 | 🌐 Lua | 📅 2023-03-10 - User-friendly framework for building your dream tabline in a few lines of code.
* [crispgm/nvim-tabline](https://github.com/crispgm/nvim-tabline) ⭐ 97 | 🐛 2 | 🌐 Lua | 📅 2024-06-03 - A port of `tabline.vim` written in Lua.
* [tomiis4/BufferTabs.nvim](https://github.com/tomiis4/BufferTabs.nvim) ⭐ 96 | 🐛 0 | 🌐 Lua | 📅 2024-08-11 - Simple and Fancy tabline.
* [johann2357/nvim-smartbufs](https://github.com/johann2357/nvim-smartbufs) ⭐ 60 | 🐛 0 | 🌐 Lua | 📅 2023-01-17 - Smart buffer management.

### Cursorline

* [nvim-mini/mini.nvim#mini.cursorword](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-cursorword.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for automatic highlighting of word under cursor (displayed after customizable delay).
* [RRethy/vim-illuminate](https://github.com/RRethy/vim-illuminate) ⭐ 2,465 | 🐛 9 | 🌐 Lua | 📅 2026-07-11 - Highlight the word under the cursor with built-in LSP support.
* [ya2s/nvim-cursorline](https://github.com/ya2s/nvim-cursorline) ⭐ 477 | 🐛 7 | 🌐 Lua | 📅 2026-02-14 - Highlights cursor words and lines.
* [mawkler/modicator.nvim](https://github.com/mawkler/modicator.nvim) ⭐ 370 | 🐛 3 | 🌐 Lua | 📅 2026-04-10 - Cursor line number mode indicator. Changes the `CursorLineNr` highlight based on Vim mode.
* [sontungexpt/stcursorword](https://github.com/sontungexpt/stcursorword) ⭐ 84 | 🐛 0 | 🌐 Lua | 📅 2025-11-30 - Highlight the word under the cursor (improved and compact version of `nvim-cursorline`).

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Startup

* [nvim-mini/mini.nvim#mini.starter](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-starter.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for start screen. Displayed items are fully customizable, item selection can be done using prefix query with instant visual feedback.
* [nvimdev/dashboard-nvim](https://github.com/nvimdev/dashboard-nvim) ⭐ 2,866 | 🐛 73 | 🌐 Lua | 📅 2026-04-17 - A minimalist dashboard, inspired by doom-emacs.
* [goolord/alpha-nvim](https://github.com/goolord/alpha-nvim) ⭐ 2,404 | 🐛 35 | 🌐 Lua | 📅 2026-04-17 - A fast and highly customizable greeter like [vim-startify](https://github.com/mhinz/vim-startify) ⭐ 5,386 | 🐛 80 | 🌐 Vim Script | 📅 2024-01-05/dashboard-nvim.
* [max397574/startup.nvim](https://github.com/max397574/startup.nvim) ⭐ 502 | 🐛 10 | 🌐 Lua | 📅 2026-06-07 - The fully customizable greeter.
* [Amansingh-afk/milli.nvim](https://github.com/Amansingh-afk/milli.nvim) ⭐ 308 | 🐛 1 | 🌐 Lua | 📅 2026-07-06 - Animated ASCII splash screens with bundled animations and custom image or GIF support.
* [CWood-sdf/spaceport.nvim](https://github.com/CWood-sdf/spaceport.nvim) ⭐ 166 | 🐛 0 | 🌐 Lua | 📅 2026-06-24 - The start screen that gets you to your projects blazingly fast.
* [TobinPalmer/Tip.nvim](https://github.com/TobinPalmer/Tip.nvim) ⭐ 82 | 🐛 1 | 🌐 Lua | 📅 2024-02-04 - Get a simple tip on startup.
* [Kurama622/profile.nvim](https://github.com/Kurama622/profile.nvim) ⭐ 78 | 🐛 0 | 🌐 Lua | 📅 2026-06-07 - A dashboard, similar to GitHub homepage.
* [mong8se/actually.nvim](https://github.com/mong8se/actually.nvim) ⭐ 66 | 🐛 2 | 🌐 Lua | 📅 2025-10-13 - Load the file you actually meant to load.
* [leo-alvarenga/homecoming.nvim](https://github.com/leo-alvarenga/homecoming.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-03-14 - A dead-simple, customizable and cozy dashboard with sane defaults and zero config required.
* [henriquehbr/nvim-startup.lua](https://sr.ht/~henriquehbr/nvim-startup.lua) - Displays the startup time.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Icon

* [nvim-mini/mini.nvim#mini.icons](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-icons.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` meant as a general icon provider. Uses fixed set of highlight groups. Supports various categories, icon and style customizations, caching for performance. Integrates with built-in filetype matching.
* [nvim-tree/nvim-web-devicons](https://github.com/nvim-tree/nvim-web-devicons) ⭐ 2,713 | 🐛 16 | 🌐 Lua | 📅 2026-07-22 - A Lua fork of [vim-devicons](https://github.com/ryanoasis/vim-devicons) ⭐ 5,806 | 🐛 70 | 🌐 Vim Script | 📅 2024-05-09.
* [2KAbhishek/nerdy.nvim](https://github.com/2KAbhishek/nerdy.nvim/) ⭐ 426 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Find and insert the latest nerd font glyphs.
* [Mirsmog/real-icons.nvim](https://github.com/Mirsmog/real-icons.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Renders PNG and SVG file icons in explorers, pickers, statuslines, and tablines through kitty's graphics protocol.
* [stephansama/fzf-nerdfont.nvim](https://github.com/stephansama/fzf-nerdfont.nvim) ⭐ 10 | 🐛 3 | 🌐 Lua | 📅 2026-01-14 - A picker for selecting Nerd Font icons using `fzf-lua`.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Media

* [3rd/image.nvim](https://github.com/3rd/image.nvim) ⭐ 2,058 | 🐛 68 | 🌐 Lua | 📅 2026-06-12 - Add image support through kitty's graphics protocol or ueberzugpp.
* [edluffy/hologram.nvim](https://github.com/edluffy/hologram.nvim) ⭐ 1,435 | 🐛 28 | 🌐 Lua | 📅 2023-11-15 - A cross platform terminal image viewer. Works on macOS and Linux.
* [HakonHarnes/img-clip.nvim](https://github.com/HakonHarnes/img-clip.nvim) ⭐ 935 | 🐛 12 | 🌐 Lua | 📅 2025-12-19 - Effortlessly embed images into any markup language, like LaTeX, Markdown or Typst.
* [vyfor/cord.nvim](https://github.com/vyfor/cord.nvim) ⭐ 691 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - Highly extensible Rich Presence for Discord.
* [ekickx/clipboard-image.nvim](https://github.com/ekickx/clipboard-image.nvim) ⭐ 336 | 🐛 9 | 🌐 Lua | 📅 2024-03-19 - Allows pasting images from clipboard.
* [davidgranstrom/scnvim](https://github.com/davidgranstrom/scnvim) ⭐ 271 | 🐛 23 | 🌐 Lua | 📅 2026-06-16 - A frontend for SuperCollider.
* [neo451/feed.nvim](https://github.com/neo451/feed.nvim) ⭐ 206 | 🐛 12 | 🌐 Lua | 📅 2026-04-01 - Web feed reader written in Lua (RSS, Atom, JSON feed).
* [adelarsq/image\_preview.nvim](https://github.com/adelarsq/image_preview.nvim) ⭐ 193 | 🐛 11 | 🌐 Lua | 📅 2026-05-06 - Image preview based on terminal's Image Protocol support.
* [Chaitanyabsrip/present.nvim](https://github.com/Chaitanyabsprip/present.nvim) ⭐ 158 | 🐛 0 | 🌐 Lua | 📅 2025-03-03 - A Presentation plugin written in Lua.
* [askfiy/nvim-picgo](https://github.com/askfiy/nvim-picgo) ⭐ 68 | 🐛 2 | 🌐 Lua | 📅 2026-03-26 - Allows you to upload images to the image bed, allowing viewing images from anywhere on the internet.
* [niuiic/code-shot.nvim](https://github.com/niuiic/code-shot.nvim) ⭐ 64 | 🐛 0 | 🌐 Lua | 📅 2025-01-04 - Take a picture of the code.
* [AntonVanAssche/music-controls.nvim](https://github.com/AntonVanAssche/music-controls.nvim) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2025-09-29 - Quickly control your favorite music player (Spotify, VLC, and more).
* [iamt4nk/smm.nvim](https://github.com/iamt4nk/smm.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2026-05-13 - Small TUI that allows for controlling Spotify playback.
* [sanjay-np/nvim-yt-player](https://github.com/sanjay-np/nvim-yt-player) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-08-12 - Play YouTube audio using `mpv` and `yt-dlp` via IPC socket.
* [melMass/echo.nvim](https://github.com/melMass/echo.nvim) ⭐ 16 | 🐛 1 | 🌐 Rust | 📅 2025-11-26 - Seamless sound integration for your editing workflow.
* [niuiic/cp-image.nvim](https://github.com/niuiic/cp-image.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Paste image from clipboard and insert the reference code.
* [ricmonmol/nvim-music-player](https://github.com/ricmonmol/nvim-music-player) ⭐ 6 | 🐛 2 | 🌐 Python | 📅 2026-01-20 - A simple music player powered by `mpv`, written in Python, including a Telescope browser.
* [T-b-t-nchos/FMP7.nvim](https://github.com/T-b-t-nchos/FMP7.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-06-10 - Control FMP7 and play FM/SSG/PCM driver music files (Only for Windows).
* [\~elisoli/nekovim](https://git.sr.ht/~elisoli/nekovim) - Flexible Discord rich presence.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Note Taking

* [nvim-neorg/neorg](https://github.com/nvim-neorg/neorg) ⭐ 7,482 | 🐛 218 | 🌐 Lua | 📅 2026-08-14 - Modernity meets insane extensibility. The future of organizing your life.
* [nvim-orgmode/orgmode](https://github.com/nvim-orgmode/orgmode) ⭐ 3,862 | 🐛 158 | 🌐 Lua | 📅 2026-06-29 - Org-mode clone written in Lua.
* [obsidian-nvim/obsidian.nvim](https://github.com/obsidian-nvim/obsidian.nvim) ⭐ 2,095 | 🐛 62 | 🌐 Lua | 📅 2026-08-14 - Plugin for Obsidian, written in Lua.
* [nvim-telekasten/telekasten.nvim](https://github.com/nvim-telekasten/telekasten.nvim) ⭐ 1,689 | 🐛 66 | 🌐 Lua | 📅 2026-03-17 - Work with a text-based, Markdown zettelkasten / wiki and mix it with a journal, based on telescope.nvim.
* [jbyuki/venn.nvim](https://github.com/jbyuki/venn.nvim) ⭐ 1,178 | 🐛 5 | 🌐 Lua | 📅 2024-08-16 - Draw ASCII diagrams.
* [zk-org/zk-nvim](https://github.com/zk-org/zk-nvim) ⭐ 848 | 🐛 0 | 🌐 Lua | 📅 2026-07-21 -  Provides integration with `zk`, a plain text note-taking assistant.
* [jakewvincent/mkdnflow.nvim](https://github.com/jakewvincent/mkdnflow.nvim) ⭐ 826 | 🐛 19 | 🌐 Lua | 📅 2026-07-03 - Fluent Markdown notebook navigation and management (create links, follow links, create and manage to-do lists, reference bib files, and more).
* [jbyuki/nabla.nvim](https://github.com/jbyuki/nabla.nvim) ⭐ 747 | 🐛 25 | 🌐 Lua | 📅 2025-04-21 - Take your scientific notes.
* [bngarren/checkmate.nvim](https://github.com/bngarren/checkmate.nvim) ⭐ 376 | 🐛 8 | 🌐 Lua | 📅 2026-05-18 - A full-featured Markdown-based TODO plugin.
* [serenevoid/kiwi.nvim](https://github.com/serenevoid/kiwi.nvim) ⚠️ Archived - A stripped down VimWiki with necessary features.
* [jghauser/papis.nvim](https://github.com/jghauser/papis.nvim) ⭐ 188 | 🐛 14 | 🌐 Lua | 📅 2025-11-19 - Manage your bibliography from within your favourite editor.
* [backdround/global-note.nvim](https://github.com/backdround/global-note.nvim) ⭐ 148 | 🐛 3 | 🌐 Lua | 📅 2024-02-14 - One global note in a floating window.
* [echaya/neowiki.nvim](https://github.com/echaya/neowiki.nvim) ⭐ 148 | 🐛 1 | 🌐 Lua | 📅 2026-04-28 - The modern vimwiki successor offering a minimal, intuitive workflow out of the box for note-taking and Getting Things Done (GTD).
* [nfrid/due.nvim](https://github.com/nfrid/due.nvim) ⭐ 116 | 🐛 0 | 🌐 Lua | 📅 2023-09-04 - Displays due for a date string as a virtual text.
* [chrsm/impulse.nvim](https://github.com/chrsm/impulse.nvim) ⭐ 101 | 🐛 3 | 🌐 MoonScript | 📅 2022-06-26 - Read Notion.so notes.
* [2KAbhishek/tdo.nvim](https://github.com/2KAbhishek/tdo.nvim) ⭐ 100 | 🐛 0 | 🌐 Lua | 📅 2025-11-20 - Fast and simple note taking.
* [apdot/doodle](https://github.com/apdot/doodle) ⭐ 97 | 🐛 0 | 🌐 Lua | 📅 2025-10-26 - A developer-centric knowledge base with project/branch scoped notes, bi-directional linking, note-tagging, graph-view, telescope integration, and Git synchronization.
* [IlyasYOY/obs.nvim](https://github.com/IlyasYOY/obs.nvim) ⭐ 93 | 🐛 0 | 🌐 Lua | 📅 2026-07-12 - Your Obsidian notes at the speed of thought.
* [0styx0/abbreinder.nvim](https://github.com/0styx0/abbreinder.nvim) ⭐ 92 | 🐛 0 | 🌐 Lua | 📅 2022-06-30 - Abbreviation reminders.
* [jameswolensky/marker-groups.nvim](https://github.com/jameswolensky/marker-groups.nvim) ⭐ 64 | 🐛 0 | 🌐 Lua | 📅 2026-06-08 - Take persistent code notes without modifying code.
* [iwe-org/iwe.nvim](https://github.com/iwe-org/iwe.nvim) ⭐ 53 | 🐛 1 | 🌐 Lua | 📅 2026-07-27 - Integration with `IWE`, an LSP designed for Markdown-based knowledge management and note-taking workflows.
* [ymic9963/mdnotes.nvim](https://github.com/ymic9963/mdnotes.nvim) ⭐ 35 | 🐛 8 | 🌐 Lua | 📅 2026-08-16 - Simple, improved, and extensible Markdown note taking.
* [lfilho/note2cal.nvim](https://github.com/lfilho/note2cal.nvim) ⭐ 29 | 🐛 1 | 🌐 Lua | 📅 2026-07-15 - Create calendar events from Markdown notes (macOS only).
* [MattHandzel/taskwarrior.nvim](https://github.com/MattHandzel/taskwarrior.nvim) ⭐ 29 | 🐛 3 | 🌐 Lua | 📅 2026-08-16 - Edit Taskwarrior tasks in a buffer, render tasks as Markdown checkboxes, bulk-edit with Vim motions, diff-and-apply on save. Inspired by oil.nvim.
* [y3owk1n/dotmd.nvim](https://github.com/y3owk1n/dotmd.nvim) ⭐ 28 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - Managing notes, TODO's, journal entries, and your inbox, all with Markdown.
* [Ostralyan/scribe.nvim](https://github.com/Ostralyan/scribe.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2023-02-02 - Take notes, easily.
* [DaFi-1/tasknvim](https://github.com/DaFi-1/tasknvim) ⭐ 20 | 🐛 1 | 🌐 Lua | 📅 2026-05-07 - A simple tool for life and personal development that helps organize goals, track habits, and improve productivity.
* [niuiic/todo.nvim](https://github.com/niuiic/todo.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2024-11-05 - Simple but powerful TODO manager based on text.
* [athar-qadri/scratchpad.nvim](https://github.com/athar-qadri/scratchpad.nvim) ⭐ 16 | 🐛 0 | 🌐 Lua | 📅 2025-03-09 - Effortlessly manage scratchpads within your favorite editor.
* [flashcodes-themayankjha/Fknotes.nvim](https://github.com/flashcodes-themayankjha/Fknotes.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-10-16 - Take notes, TODOs from anywhere inside your project, search all TODOs, get reminders and more.
* [slugbyte/whip.nvim](http://github.com/slugbyte/whip.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2025-04-03 - A super fast minimal scratchpad management plugin, biew biew biew.
* [happyeric77/joplin.nvim](https://github.com/happyeric77/joplin.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2025-09-07 - Joplin notes utilities: tree browser, search, open, and Telescope integration.
* [gmcusaro/ma.nvim](https://github.com/gmcusaro/ma.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-03-22 - Minimal Markdown knowledge management with relational note navigation and safe file operations.
* [jjuchara/obsidian-tasks.nvim](https://github.com/jjuchara/obsidian-tasks.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-08-12 - Keyboard-first Obsidian task management across multiple vaults with ordered tag trees.
* [indium114/studytools.nvim](https://github.com/indium114/studytools.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-03-27 - Various utilities to enhance the studying and note-taking experience.
* [nbeversl/urtext\_neovim](https://github.com/nbeversl/urtext_neovim) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2026-04-29 - An implementation of Urtext.
* [carloscalla/notepad.nvim](https://github.com/carloscalla/notepad.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-01-27 - Quick note-taking in Markdown with both repo-specific and global notepad support.
* [sduras/duras\_bridge](https://github.com/sduras/duras_bridge) - Bridge for [duras](https://codeberg.org/duras/duras) plain-text daily notes; append, search, and open notes from the editor.
* [losch/ztl](https://codeberg.org/losch/ztl) - A fast static note generator in a single binary with everything built-in.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Utility

* [jbyuki/instant.nvim](https://github.com/jbyuki/instant.nvim) ⭐ 1,417 | 🐛 9 | 🌐 Lua | 📅 2022-12-31 - A collaborative editing plugin written in Lua with no dependencies.
* [mistricky/codesnap.nvim](https://github.com/mistricky/codesnap.nvim) ⭐ 927 | 🐛 29 | 🌐 Lua | 📅 2026-08-10 - Snapshot plugin with rich features that can make pretty code snapshots.
* [code-biscuits/nvim-biscuits](https://github.com/code-biscuits/nvim-biscuits) ⭐ 345 | 🐛 6 | 🌐 Lua | 📅 2026-03-23 - A port of Assorted Biscuits. Ends up with more supported languages too.
* [axieax/urlview.nvim](https://github.com/axieax/urlview.nvim) ⭐ 281 | 🐛 7 | 🌐 Lua | 📅 2025-11-30 - Browse all URLs in the current buffer.
* [LintaoAmons/scratch.nvim](https://github.com/LintaoAmons/scratch.nvim) ⭐ 278 | 🐛 9 | 🌐 Lua | 📅 2026-05-26 - Create and manage scratch files.
* [Owen-Dechow/videre.nvim](https://github.com/Owen-Dechow/videre.nvim) ⭐ 271 | 🐛 8 | 🌐 Lua | 📅 2026-06-24 - Explore JSON, YAML, and TOML files as nested unit/node-based graphical representations.
* [crusj/bookmarks.nvim](https://github.com/crusj/bookmarks.nvim) ⭐ 248 | 🐛 10 | 🌐 Lua | 📅 2024-07-12 - Remember file locations and sort by time and frequency.
* [chrisgrieser/nvim-genghis](https://github.com/chrisgrieser/nvim-genghis) ⭐ 222 | 🐛 2 | 🌐 Lua | 📅 2026-08-03 - Convenience file operations, written in Lua.
* [subnut/nvim-ghost.nvim](https://github.com/subnut/nvim-ghost.nvim) ⭐ 199 | 🐛 14 | 🌐 Python | 📅 2026-05-15 - GhostText support with zero dependencies.
* [philosofonusus/ecolog.nvim](https://github.com/philosofonusus/ecolog.nvim) ⭐ 171 | 🐛 3 | 🌐 Lua | 📅 2026-02-02 - Sophisticated all-in-one toolkit to work with `.env` files and environment variables.
* [mluders/comfy-line-numbers.nvim](https://github.com/mluders/comfy-line-numbers.nvim) ⭐ 138 | 🐛 10 | 🌐 Lua | 📅 2026-01-26 - Limits relative numbers to only show left-hand digits on the keyboard.
* [sontungexpt/url-open](https://github.com/sontungexpt/url-open) ⭐ 108 | 🐛 10 | 🌐 Lua | 📅 2025-10-29 - Open URLs under the cursor and create highlight effects for them.
* [rktjmp/paperplanes.nvim](https://github.com/rktjmp/paperplanes.nvim) ⭐ 99 | 🐛 0 | 🌐 Fennel | 📅 2025-07-14 - Post selections or buffers to online paste bins.
* [ysmb-wtsg/in-and-out.nvim](https://github.com/ysmb-wtsg/in-and-out.nvim) ⭐ 90 | 🐛 0 | 🌐 Lua | 📅 2025-08-16 - Quick navigation in and out of surrounding characters.
* [y3owk1n/time-machine.nvim](https://github.com/y3owk1n/time-machine.nvim) ⭐ 80 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - Take control of your edit history with an interactive timeline, diff previews, taggings, live reloading trees and cleanup functions.
* [gpanders/nvim-moonwalk](https://github.com/gpanders/nvim-moonwalk) ⭐ 77 | 🐛 0 | 🌐 Lua | 📅 2022-04-12 - Use any language that compiles to Lua anywhere in your configuration.
* [doctorfree/cheatsheet.nvim](https://github.com/doctorfree/cheatsheet.nvim) ⭐ 74 | 🐛 6 | 🌐 Lua | 📅 2025-10-31 - Searchable cheatsheet.
* [josephburgess/nvumi](https://github.com/josephburgess/nvumi) ⭐ 72 | 🐛 1 | 🌐 Lua | 📅 2026-04-09 - Natural language calculator in a scratch buffer.
* [figsoda/nix-develop.nvim](https://github.com/figsoda/nix-develop.nvim) ⭐ 70 | 🐛 0 | 🌐 Lua | 📅 2026-01-29 - Run `nix develop` without restarting.
* [necrom4/calcium.nvim](https://github.com/necrom4/calcium.nvim) ⭐ 67 | 🐛 0 | 🌐 Lua | 📅 2025-12-27 - A powerful [`lua-lib-math`](https://www.lua.org/pil/18.html) in-buffer calculator with visual mode, functions and variable support.
* [zeybek/camouflage.nvim](https://github.com/zeybek/camouflage.nvim) ⭐ 61 | 🐛 2 | 🌐 Lua | 📅 2026-07-06 - Hide sensitive values in configuration files during screen sharing by visually masking secrets in `.env`, `.json`, `.yaml`, `.toml`, and `.properties` files.
* [paulburgess1357/nvim-mcp](https://github.com/paulburgess1357/nvim-mcp) ⭐ 60 | 🐛 0 | 🌐 Python | 📅 2026-08-06 - MCP server giving AI agents access to buffers, commands, and LSP diagnostics through the built-in msgpack-RPC socket.
* [ellisonleao/dotenv.nvim](https://github.com/ellisonleao/dotenv.nvim) ⭐ 59 | 🐛 3 | 🌐 Lua | 📅 2025-03-27 - Minimalist `.env` support.
* [redoxahmii/json-to-types.nvim](https://github.com/redoxahmii/json-to-types.nvim) ⭐ 59 | 🐛 0 | 🌐 Lua | 📅 2026-02-18 - Convert JSON objects to type definitions for multiple languages.
* [MisanthropicBit/decipher.nvim](https://github.com/MisanthropicBit/decipher.nvim) ⭐ 47 | 🐛 3 | 🌐 Lua | 📅 2026-05-22 - Encode and decode text using various codecs such as base64.
* [terje/simctl.nvim](https://github.com/terje/simctl.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2024-12-15 - Interact with iOS Simulators.
* [0xJohnnyboy/scretch.nvim](https://github.com/0xJohnnyboy/scretch.nvim) ⭐ 38 | 🐛 0 | 🌐 Lua | 📅 2026-08-06 - Create and manage scratch files, scratch templates, with picker integrations.
* [yutkat/confirm-quit.nvim](https://github.com/yutkat/confirm-quit.nvim) ⭐ 38 | 🐛 0 | 🌐 Lua | 📅 2025-04-25 - Confirm before quitting.
* [ovk/endec.nvim](https://github.com/ovk/endec.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2025-04-07 - Encode, decode and re-encode text using Base64, Base64URL and URL (percent) encodings.
* [tenxsoydev/nx.nvim](https://github.com/tenxsoydev/nx.nvim) ⭐ 33 | 🐛 5 | 🌐 Lua | 📅 2024-10-17 - Built-in API utility wrapper for more convenience with Lua keymaps, highlights, autocommands and options.
* [AlejandroSuero/freeze-code.nvim](https://github.com/AlejandroSuero/freeze-code.nvim) ⭐ 32 | 🐛 3 | 🌐 Lua | 📅 2025-03-15 - Code screenshot plugin that makes use of [freeze](https://github.com/charmbracelet/freeze) ⭐ 4,785 | 🐛 78 | 🌐 Go | 📅 2026-08-13 inside the editor.
* [emrearmagan/dockyard.nvim](https://github.com/emrearmagan/dockyard.nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2026-05-18 - Docker dashboard for managing containers, images, networks, and logs.
* [linrongbin16/gentags.nvim](https://github.com/linrongbin16/gentags.nvim) ⭐ 24 | 🐛 1 | 🌐 Lua | 📅 2025-08-20 - The tags generator/management for old school vimers.
* [aPeoplesCalendar/apc.nvim](https://github.com/aPeoplesCalendar/apc.nvim) ⭐ 23 | 🐛 2 | 🌐 Lua | 📅 2024-06-18 - "On this day" style calendar, which provides information about worldwide history of working class movements and liberation struggles.
* [bgaillard/readonly.nvim](https://github.com/bgaillard/readonly.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-07-11 - Secure edition of files containing sensible / secret information, passwords, API keys, SSH keys, etc.
* [gaborvecsei/cryptoprice.nvim](https://github.com/gaborvecsei/cryptoprice.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - Check the price of the defined cryptocurrencies.
* [ragnarok22/whereami.nvim](https://github.com/ragnarok22/whereami.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2026-07-10 - Test your VPN by getting you current location.
* [johannww/tts.nvim](https://github.com/johannww/tts.nvim) ⭐ 21 | 🐛 1 | 🌐 Lua | 📅 2025-11-26 - Text to speech tool based on the Microsoft Edge online services.
* [piersolenski/brewfile.nvim](https://github.com/piersolenski/brewfile.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-11-03 - Manage your [Homebrew](https://brew.sh/) [Brewfile](https://docs.brew.sh/Brew-Bundle-and-Brewfile).
* [glyccogen/imprint.nvim](https://github.com/glyccogen/imprint.nvim) ⭐ 18 | 🐛 2 | 🌐 Lua | 📅 2026-02-15 - Take WYSIWYG screenshots of your code via Playwright and headless Chromium, preserving your colorscheme and highlights.
* [athar-qadri/weather.nvim](https://github.com/athar-qadri/weather.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-07-27 - Realtime weather and earthquake alerts with support for lualine integration (no API key required).
* [wsdjeg/ctags.nvim](https://github.com/wsdjeg/ctags.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2026-07-17 - Generate tags files and update tags option automatically.
* [ChuYanLon/telegram.nvim](https://github.com/ChuYanLon/telegram.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-08-09 - A Telegram chat client powered by TDLib supporting real-time messaging, group management, and media preview.
* [leblocks/toggle.nvim](https://github.com/leblocks/toggle.nvim) ⭐ 13 | 🐛 1 | 🌐 Lua | 📅 2026-06-14 - Toggle between common words under the cursor such as *public* ⇄ *private* ⇄ *protected*. Easy to add and overwrite built-in toggles.
* [indium114/unobtrusive-relnums.nvim](https://github.com/indium114/unobtrusive-relnums.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-06-26 - Unobtrusive relative line numbers in the sign column.
* [theKnightsOfRohan/hexer.nvim](https://github.com/theKnightsOfRohan/hexer.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-04-28 - Easily convert between binary representations without a conversion table.
* [indium114/cheaty.nvim](https://github.com/indium114/cheaty.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-03-27 - A simple, configurable cheatsheet.
* [Zeioth/distroupdate.nvim](https://github.com/Zeioth/distroupdate.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2025-08-11 - Distro agnostic updater to get the latest changes from the Git repository of your config.
* [wsdjeg/mru.nvim](https://github.com/wsdjeg/mru.nvim) ⭐ 10 | 🐛 1 | 🌐 Lua | 📅 2026-07-14 - Manage and display your Most Recently Used (MRU) files.
* [dpezto/chezmoi-template.nvim](https://github.com/dpezto/chezmoi-template.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-08-12 - Edit chezmoi source files natively: target-language Tree-sitter injection, template-aware formatting, live preview, diagnostics and completion.
* [StefanBartl/color\_my\_ascii.nvim](https://github.com/StefanBartl/color_my_ascii.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-08-15 - Colorful highlighting of ASCII art in Markdown code blocks.
* [leo-alvarenga/quoth.nvim](https://github.com/leo-alvarenga/quoth.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2025-12-17 - A lightweight, configurable random quote provider with lazy loading, custom tables, and filters.
* [mahyarmirrashed/famous-quotes.nvim](https://github.com/mahyarmirrashed/famous-quotes.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-03-11 - Get famous quotes from history to display on startup.
* [cxwx/lazyUrlUpdate.nvim](https://github.com/cxwx/lazyUrlUpdate.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-07-21 - Update plugin under cursor by `lazy.nvim`.
* [penaz91/MiniDYM](https://github.com/Penaz91/MiniDYM) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - A very small "Did you mean" plugin, suggesting files the user might have wanted to open instead of creating a new one.
* [iquzart/toggleword.nvim](https://github.com/iquzart/toggleword.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-07-25 - Toggle between common code keywords under the cursor such as true ⇄ false, on ⇄ off, enabled ⇄ disabled, and dev ⇄ prod.

### CSV Files

* [hat0uma/csvview.nvim](https://github.com/hat0uma/csvview.nvim) ⭐ 676 | 🐛 17 | 🌐 Lua | 📅 2026-05-02 - An asynchronous CSV/TSV table viewer with real-time updates, configurable comments and delimiters, and multiple display modes.
* [emmanueltouzery/decisive.nvim](https://github.com/emmanueltouzery/decisive.nvim) ⭐ 128 | 🐛 1 | 🌐 Lua | 📅 2026-06-06 - View and edit CSV files with ease and speed.
* [VidocqH/data-viewer.nvim](https://github.com/VidocqH/data-viewer.nvim) ⭐ 124 | 🐛 9 | 🌐 Lua | 📅 2024-07-29 - Provide a simple table view to inspect data files such as `csv`, `tsv`.
* [theKnightsOfRohan/csvlens.nvim](https://github.com/theKnightsOfRohan/csvlens.nvim) ⭐ 40 | 🐛 1 | 🌐 Lua | 📅 2024-04-28 - A port of [YS-L/csvlens](https://github.com/YS-L/csvlens) ⭐ 3,933 | 🐛 57 | 🌐 Rust | 📅 2026-07-04, for easy previewing of tabular data.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Animation

* [nvim-mini/mini.nvim#mini.animate](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-animate.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to add out of the box animations for common built-in actions (cursor movement, scroll, resize, window open/close).
* [sphamba/smear-cursor.nvim](https://github.com/sphamba/smear-cursor.nvim) ⭐ 1,987 | 🐛 8 | 🌐 Lua | 📅 2026-04-15 - Animate the cursor with a smear effect in all terminals. Inspired by Neovide's animated cursor.
* [rachartier/tiny-glimmer.nvim](https://github.com/rachartier/tiny-glimmer.nvim/) ⭐ 431 | 🐛 1 | 🌐 Lua | 📅 2026-07-05 - Adds subtle animations to various operations.
* [gen740/SmoothCursor.nvim](https://github.com/gen740/SmoothCursor.nvim) ⭐ 402 | 🐛 3 | 🌐 Lua | 📅 2024-09-18 - Add fancy sub-cursor to signcolumn to show your scroll or jump direction.
* [y3owk1n/undo-glow.nvim](https://github.com/y3owk1n/undo-glow.nvim/) ⭐ 104 | 🐛 1 | 🌐 Lua | 📅 2026-07-04 - Animated glow/highlight effects for editing operations (undo, redo, yank, paste, etc.) with fully customizable animations and appearance.
* [LuxVim/nvim-luxmotion](https://github.com/LuxVim/nvim-luxmotion) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2026-07-08 - Smooth, high‑performance motion and scrolling animations — 60fps fluid cursor moves, word jumps, and viewport scrolling, all in one.
* [indium114/smudge.nvim](https://github.com/indium114/smudge.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-03-27 - Performant cursor animations.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Terminal Integration

* [akinsho/toggleterm.nvim](https://github.com/akinsho/toggleterm.nvim) ⭐ 5,582 | 🐛 92 | 🌐 Lua | 📅 2025-03-09 - Easily manage multiple terminal windows.
* [kassio/neoterm](https://github.com/kassio/neoterm) ⭐ 1,341 | 🐛 31 | 🌐 Vim Script | 📅 2023-03-09 - Wrapper of some `:terminal` functions.
* [mikesmithgh/kitty-scrollback.nvim](https://github.com/mikesmithgh/kitty-scrollback.nvim) ⭐ 906 | 🐛 28 | 🌐 Lua | 📅 2026-08-13 - Open your kitty scrollback buffer. Ameowzing.
* [numToStr/FTerm.nvim](https://github.com/numToStr/FTerm.nvim) ⭐ 813 | 🐛 30 | 🌐 Lua | 📅 2023-10-19 - No nonsense floating terminal written in Lua.
* [willothy/flatten.nvim](https://github.com/willothy/flatten.nvim) ⭐ 726 | 🐛 16 | 🌐 Lua | 📅 2026-06-19 - Open files from terminal buffers in your current editor instance instead of launching a nested instance.
* [nikvdp/neomux](https://github.com/nikvdp/neomux) ⭐ 391 | 🐛 1 | 🌐 Vim Script | 📅 2026-06-27 - Control your editor from shells ran through the `:term` command.
* [norcalli/nvim-terminal.lua](https://github.com/norcalli/nvim-terminal.lua) ⭐ 296 | 🐛 7 | 🌐 Lua | 📅 2022-11-21 - A high performance filetype mode which leverages conceal and highlights your buffer with the correct color codes.
* [samjwill/nvim-unception](https://github.com/samjwill/nvim-unception) ⭐ 245 | 🐛 9 | 🌐 Lua | 📅 2026-05-14 - Automatic unnesting of editor sessions started from terminal buffers.
* [chomosuke/term-edit.nvim](https://github.com/chomosuke/term-edit.nvim) ⭐ 214 | 🐛 8 | 🌐 Lua | 📅 2024-10-17 - Allowing you to edit your command in the terminal just like any other buffer.
* [laktak/tome](https://github.com/laktak/tome) ⭐ 175 | 🐛 1 | 🌐 Vim Script | 📅 2026-08-13 - Interactive Script playbooks for your terminal (optionally with Tmux).
* [s1n7ax/nvim-terminal](https://github.com/s1n7ax/nvim-terminal) ⭐ 118 | 🐛 2 | 🌐 Lua | 📅 2026-02-10 - A simple and easy to use multi-terminal plugin.
* [samharju/yeet.nvim](https://github.com/samharju/yeet.nvim) ⭐ 118 | 🐛 1 | 🌐 Lua | 📅 2026-03-04 - Run shell commands in terminal buffers or tmux panes.
* [jghauser/kitty-runner.nvim](https://github.com/jghauser/kitty-runner.nvim) ⭐ 112 | 🐛 8 | 🌐 Lua | 📅 2026-03-27 - Poor man's REPL. Easily send buffer lines and commands to a kitty terminal.
* [waiting-for-dev/ergoterm.nvim](https://github.com/waiting-for-dev/ergoterm.nvim) ⭐ 105 | 🐛 0 | 🌐 Lua | 📅 2026-06-17 - Seamless terminal workflow integration with smart picker-based terminal selection, flexible text sending and persistent configuration.
* [2KAbhishek/termim.nvim](https://github.com/2KAbhishek/termim.nvim/) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2025-12-01 - Built-in terminal, improved.
* [Dan7h3x/neaterm.nvim](https://github.com/Dan7h3x/neaterm.nvim) ⭐ 76 | 🐛 1 | 🌐 Lua | 📅 2026-06-25 - A little smart terminal/REPL manager with awesome features.
* [nyngwang/NeoTerm.lua](https://github.com/nyngwang/NeoTerm.lua) ⭐ 69 | 🐛 7 | 🌐 Lua | 📅 2024-01-27 - Attach a terminal for each **buffer**, now with stable toggle and astonishing cursor restoring.
* [jlesquembre/nterm.nvim](https://github.com/jlesquembre/nterm.nvim) ⭐ 58 | 🐛 1 | 🌐 Lua | 📅 2026-08-11 - Interact with the terminal, with notifications.
* [isak102/ghostty.nvim](https://github.com/isak102/ghostty.nvim) ⭐ 48 | 🐛 1 | 🌐 Lua | 📅 2025-01-04 - Automatically validate your Ghostty configuration on save.
* [da-moon/telescope-toggleterm.nvim](https://github.com/da-moon/telescope-toggleterm.nvim) ⭐ 39 | 🐛 0 | 🌐 Dockerfile | 📅 2022-02-09 - Telescope picker for terminal buffers.
* [ingur/floatty.nvim](https://github.com/ingur/floatty.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2026-07-05 - A tiny (<200 LOC) but highly customizable floating terminal manager.
* [logicmagix/tide42](https://github.com/logicmagix/tide42) ⭐ 28 | 🐛 0 | 🌐 Shell | 📅 2026-07-20 - A fully integrated terminal IDE built on Lua, tmux, and scriptable workflows.
* [benoror/gpg.nvim](https://github.com/benoror/gpg.nvim) ⭐ 22 | 🐛 1 | 🌐 Lua | 📅 2026-08-07 - Edit GPG encrypted files symmetrically.
* [niuiic/terminal.nvim](https://github.com/niuiic/terminal.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2024-11-13 - Manage terminal as buffer, multiple terminals support.
* [NeViRAIDE/nekifoch.nvim](https://github.com/NeViRAIDE/nekifoch.nvim) ⚠️ Archived - Managing kitty terminal font settings.
* [LuxVim/nvim-luxterm](https://github.com/LuxVim/nvim-luxterm) ⭐ 15 | 🐛 2 | 🌐 Lua | 📅 2026-06-09 - A floating-window terminal session manager, offering elegant multi-terminal organization, live previews, and intuitive navigation with modern UI design. Manage, switch, and customize multiple terminals effortlessly.
* [imranzero/multiterm.nvim](https://github.com/imranZERO/multiterm.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-06-06 - Effortlessly manage multiple floating terminal windows.
* [TheLazyCat00/runner-nvim](https://github.com/TheLazyCat00/runner-nvim) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2026-02-11 - Run commands in a floating terminal and keep track of the last command executed per CWD, making it easy to repeat build or test commands.
* [idanarye/nvim-channelot](https://github.com/idanarye/nvim-channelot) ⭐ 8 | 🐛 2 | 🌐 Lua | 📅 2025-10-26 - Operate editor jobs from Lua coroutines.
* [gh-liu/nvim-winterm](https://github.com/gh-liu/nvim-winterm) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-01-29 - Multi-terminal window manager.
* [Senal-D-A-Gunaratna/hyprfade.nvim](https://github.com/Senal-D-A-Gunaratna/hyprfade.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - When using Hyprland, fade the terminal window via `hyprctl`.
* [hawknewton/termyank.nvim](https://github.com/hawknewton/termyank.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-05-12 - Avoid yanking newlines in a terminal buffer.
* [TheLazyCat00/termfile-nvim](https://github.com/TheLazyCat00/termfile-nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-07-22 - Turn files into persistent terminal sessions that flawlessly allow for background work.
* [Axot017/multiterm.nvim](https://github.com/Axot017/multiterm.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2025-04-29 - A lightweight manager of multiple terminal instances with key bindings.
* [jaimeibanezrivera/zj-theme](https://github.com/jaimeibanezrivera/zj-theme) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-07-30 - Syncs zellij's theme to whatever colorscheme is active, live, no restart needed.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Debugging

* [mfussenegger/nvim-dap](https://github.com/mfussenegger/nvim-dap) ⭐ 7,222 | 🐛 32 | 🌐 Lua | 📅 2026-06-20 - Debug Adapter Protocol client implementation.
* [rcarriga/nvim-dap-ui](https://github.com/rcarriga/nvim-dap-ui) ⭐ 3,365 | 🐛 108 | 🌐 Lua | 📅 2026-07-14 - A UI for nvim-dap.
* [theHamsta/nvim-dap-virtual-text](https://github.com/theHamsta/nvim-dap-virtual-text) ⭐ 1,083 | 🐛 12 | 🌐 Lua | 📅 2025-05-25 - Virtual text support for nvim-dap.
* [igorlfs/nvim-dap-view](https://github.com/igorlfs/nvim-dap-view) ⭐ 985 | 🐛 11 | 🌐 Lua | 📅 2026-08-11 - A modern, minimalistic UI for nvim-dap.
* [sakhnik/nvim-gdb](https://github.com/sakhnik/nvim-gdb) ⭐ 783 | 🐛 5 | 🌐 Lua | 📅 2026-06-15 - Thin wrapper for GDB, LLDB, PDB/PDB++ and BashDB.
* [andrewferrier/debugprint.nvim](https://github.com/andrewferrier/debugprint.nvim) ⭐ 526 | 🐛 9 | 🌐 Lua | 📅 2026-07-04 - Debugging the print() way.
* [pocco81/dap-buddy.nvim](https://github.com/pocco81/dap-buddy.nvim) ⭐ 394 | 🐛 25 | 🌐 Lua | 📅 2022-09-26 - Manage several debuggers for nvim-dap.
* [t-troebst/perfanno.nvim](https://github.com/t-troebst/perfanno.nvim) ⭐ 369 | 🐛 1 | 🌐 Lua | 📅 2026-01-20 - Annotate your code with callgraph profiling data. Native support for perf, flamegraph and the LuaJIT profiler.
* [Weissle/persistent-breakpoints.nvim](https://github.com/Weissle/persistent-breakpoints.nvim) ⭐ 260 | 🐛 2 | 🌐 Lua | 📅 2025-03-22 - Persistent breakpoints for nvim-dap.
* [chrisgrieser/nvim-chainsaw](https://github.com/chrisgrieser/nvim-chainsaw) ⭐ 140 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Speed up log creation. Creates various kinds of language-specific log statements, like logs of variables, assertions, or time-measuring.
* [NickTsaizer/splitasm.nvim](https://github.com/NickTsaizer/splitasm.nvim) ⭐ 78 | 🐛 0 | 🌐 Lua | 📅 2026-05-16 - View compiled assembly output side by side with source code, with synchronized cursor movement.
* [niuiic/dap-utils](https://github.com/niuiic/dap-utils.nvim) ⭐ 41 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Utilities to provide a better experience for using nvim-dap.
* [Willem-J-an/visidata.nvim](https://github.com/Willem-J-an/visidata.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2024-03-19 - Render Pandas dataframes in `nvim-dap` using the power of visidata.
* [ofirgall/goto-breakpoints.nvim](https://github.com/ofirgall/goto-breakpoints.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2023-11-02 - Cycle between breakpoints for nvim-dap.
* [Carcuis/dap-breakpoints.nvim](https://github.com/Carcuis/dap-breakpoints.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2026-01-09 - Manage and create advanced breakpoints with virtual text and popup reveal for nvim-dap.
* [ravsii/nvim-dap-envfile](https://github.com/ravsii/nvim-dap-envfile) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-01-10 - Automatic `envFile` support for nvim-dap.
* [fschaal/azfunc.nvim](https://github.com/fschaal/azfunc.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-11-09 - Seamlessly debug Azure Functions with automatic DAP integration.
* [evanmcpheron/rocketlog.nvim](https://github.com/evanmcpheron/rocketlog.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2026-05-08 - Seamlessly add logging for JavaScript and TypeScript files, with log and metadata searching.

### Quickfix

* [kevinhwang91/nvim-bqf](https://github.com/kevinhwang91/nvim-bqf) ⭐ 2,029 | 🐛 21 | 🌐 Lua | 📅 2026-04-02 - Makes the quickfix window better.
* [stevearc/quicker.nvim](https://github.com/stevearc/quicker.nvim) ⭐ 1,024 | 🐛 19 | 🌐 Lua | 📅 2026-05-24 - Improved quickfix UI and editable quickfix buffer.
* [yorickpeterse/nvim-pqf](https://github.com/yorickpeterse/nvim-pqf) ⭐ 187 | 🐛 1 | 🌐 Lua | 📅 2026-06-10 - Prettier quickfix/location list windows.
* [ashfinal/qfview.nvim](https://github.com/ashfinal/qfview.nvim) ⭐ 54 | 🐛 1 | 🌐 Lua | 📅 2023-09-09 - Pretty quickfix/location view with consistent path-shorten and folding.
* [niuiic/quickfix.nvim](https://github.com/niuiic/quickfix.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2024-11-01 - Extended functionality for quickfix, including store, restore, make, remove, etc.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Test

* [nvim-neotest/neotest](https://github.com/nvim-neotest/neotest) ⭐ 3,108 | 🐛 102 | 🌐 Lua | 📅 2026-07-24 - An extensible framework for interacting with tests within your editor.
* [andythigpen/nvim-coverage](https://github.com/andythigpen/nvim-coverage) ⭐ 435 | 🐛 18 | 🌐 Lua | 📅 2024-12-18 - Displays coverage information in the sign column.
* [David-Kunz/jester](https://github.com/David-Kunz/jester) ⭐ 213 | 🐛 4 | 🌐 Lua | 📅 2025-01-15 - Easily run and debug Jest tests.
* [klen/nvim-test](https://github.com/klen/nvim-test) ⭐ 200 | 🐛 3 | 🌐 Lua | 📅 2026-05-16 - A wrapper for running tests.
* [nvim-neotest/neotest-jest](https://github.com/nvim-neotest/neotest-jest) ⭐ 153 | 🐛 4 | 🌐 Lua | 📅 2026-04-02 - Neotest adapter for running Jest tests.
* [quolpr/quicktest.nvim](https://github.com/quolpr/quicktest.nvim) ⭐ 104 | 🐛 4 | 🌐 C++ | 📅 2026-05-02 - Run your tests in split window or popup with live feedback.
* [MisanthropicBit/neotest-busted](https://github.com/MisanthropicBit/neotest-busted) ⭐ 18 | 🐛 7 | 🌐 Lua | 📅 2026-04-02 - Neotest adapter for running busted tests using your editor as a Lua interpreter.
* [mr-u0b0dy/crazy-coverage.nvim](https://github.com/mr-u0b0dy/crazy-coverage.nvim) ⭐ 18 | 🐛 3 | 🌐 Lua | 📅 2026-05-25 - Display code coverage.
* [zkucekovic/tdd.nvim](https://github.com/zkucekovic/tdd.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-11-05 - Opens or creates the matching PHPUnit test file for a given class, based on PSR-4 namespace mappings.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Code Runner

* [stevearc/overseer.nvim](https://github.com/stevearc/overseer.nvim) ⭐ 1,915 | 🐛 84 | 🌐 Lua | 📅 2026-05-24 - A task runner and job management plugin.
* [michaelb/sniprun](https://github.com/michaelb/sniprun) ⭐ 1,710 | 🐛 11 | 🌐 Rust | 📅 2026-07-29 - Run parts of code of any language directly from your editor.
* [Vigemus/iron.nvim](https://github.com/Vigemus/iron.nvim) ⭐ 1,358 | 🐛 56 | 🌐 Lua | 📅 2026-07-27 - Interactive REPLs of over 30 languages embedded.
* [benlubas/molten-nvim](https://github.com/benlubas/molten-nvim) ⭐ 1,207 | 🐛 40 | 🌐 Python | 📅 2026-07-03 - Enables running code chunks via the Jupyter kernel. Output (including image output) is rendered in a floating window below the code.
* [rafcamlet/nvim-luapad](https://github.com/rafcamlet/nvim-luapad) ⭐ 693 | 🐛 5 | 🌐 Lua | 📅 2026-03-23 - Interactive scratchpad for running Lua code.
* [CRAG666/code\_runner.nvim](https://github.com/CRAG666/code_runner.nvim) ⭐ 692 | 🐛 2 | 🌐 Lua | 📅 2026-07-20 - The best code runner you could have, with super powers.
* [Zeioth/compiler.nvim](https://github.com/Zeioth/compiler.nvim) ⭐ 671 | 🐛 9 | 🌐 Lua | 📅 2025-08-14 - Compiler for building and running your code without having to configure anything.
* [Civitasv/cmake-tools.nvim](https://github.com/Civitasv/cmake-tools.nvim) ⭐ 556 | 🐛 19 | 🌐 Lua | 📅 2026-06-19 - CMake integration.
* [milanglacier/yarepl.nvim](https://github.com/milanglacier/yarepl.nvim) ⭐ 251 | 🐛 2 | 🌐 Lua | 📅 2026-08-02 - Yet Another REPL, flexible, supporting multiple paradigms to interact with REPLs, and native dot repeat without other dependencies.
* [EthanJWright/vs-tasks.nvim](https://github.com/EthanJWright/vs-tasks.nvim) ⭐ 214 | 🐛 0 | 🌐 Lua | 📅 2025-10-27 - Run and manage project jobs, supporting VSCode's `tasks.json` spec.
* [krady21/compiler-explorer.nvim](https://github.com/krady21/compiler-explorer.nvim) ⭐ 194 | 🐛 2 | 🌐 Lua | 📅 2026-02-09 - Asynchronous compilation using the [compiler-explorer](https://godbolt.org/) REST API.
* [is0n/jaq-nvim](https://github.com/is0n/jaq-nvim) ⭐ 179 | 🐛 10 | 🌐 Lua | 📅 2024-07-21 - Just Another Quickrun Plugin in Lua.
* [jedrzejboczar/toggletasks.nvim](https://github.com/jedrzejboczar/toggletasks.nvim) ⭐ 162 | 🐛 5 | 🌐 Lua | 📅 2023-03-08 - Task runner with JSON/YAML configs, using toggleterm.nvim and telescope.nvim.
* [google/executor.nvim](https://github.com/google/executor.nvim) ⭐ 159 | 🐛 10 | 🌐 Lua | 📅 2025-08-15 - Allows you to run command line tasks in the background and be notified of results.
* [Shatur/neovim-tasks](https://github.com/Shatur/neovim-tasks) ⭐ 129 | 🐛 4 | 🌐 Lua | 📅 2026-07-01 - A stateful task manager focused on integration with build systems.
* [MarcHamamji/runner.nvim](https://github.com/MarcHamamji/runner.nvim) ⭐ 52 | 🐛 2 | 🌐 Lua | 📅 2025-03-04 - A customizable Lua code runner.
* [dasupradyumna/launch.nvim](https://github.com/dasupradyumna/launch.nvim) ⭐ 50 | 🐛 14 | 🌐 Lua | 📅 2025-07-06 - A simple and quick task launcher which allows dynamically configuring tasks on the fly, with optional support for debugging.
* [al1-ce/just.nvim](https://github.com/al1-ce/just.nvim) ⭐ 49 | 🐛 6 | 🌐 Lua | 📅 2026-02-14 - Task runner for justfiles.
* [Zeioth/makeit.nvim](https://github.com/Zeioth/makeit.nvim) ⭐ 48 | 🐛 7 | 🌐 Lua | 📅 2025-06-24 - Makefile runner based on overseer.
* [chrisgrieser/nvim-justice](https://github.com/chrisgrieser/nvim-justice) ⭐ 37 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Lightweight integration of the `just` task runner.
* [wsdjeg/tasks.nvim](https://github.com/wsdjeg/tasks.nvim) ⭐ 32 | 🐛 1 | 🌐 Lua | 📅 2026-07-17 - A tasks manager that integrates with external tools, inspired by VSCode's tasks-manager.
* [desdic/greyjoy.nvim](https://github.com/desdic/greyjoy.nvim) ⭐ 31 | 🐛 0 | 🌐 Lua | 📅 2025-12-24 - A modular task runner for Makefiles, VSCode tasks, kitchen etc.
* [pianocomposer321/officer.nvim](https://github.com/pianocomposer321/officer.nvim) ⭐ 23 | 🐛 3 | 🌐 Lua | 📅 2026-05-17 - Like dispatch.vim but using overseer.nvim.
* [idanarye/nvim-moonicipal](https://github.com/idanarye/nvim-moonicipal) ⭐ 20 | 🐛 1 | 🌐 Lua | 📅 2025-11-03 - Task runner with focus on rapidly changing personal tasks.
* [ok97465/ipybridge.nvim](https://github.com/ok97465/ipybridge.nvim) ⭐ 13 | 🐛 4 | 🌐 Lua | 📅 2026-03-20 - Run Python code, execute Jupyter cells, debug, and explore variables.
* [hadishahpuri/nvimlaunch](https://github.com/hadishahpuri/nvimlaunch) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2026-07-20 - Define, run, and manage project-specific commands.
* [jaytyrrell13/static.nvim](https://github.com/jaytyrrell13/static.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2023-12-29 - Run static site generator commands.
* [pewpewnor/pilot.nvim](https://github.com/pewpewnor/pilot.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-08-09 - Run your projects and files quickly with keybindings, and configure how to run them on the fly.
* [lewistg/pesto.nvim](https://github.com/lewistg/pesto.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-07-14 - - Bazel integration through its *Build Event Protocol* to find, fetch, and parse error logs for failed build actions, including logs stored remotely.
* [speelbarrow/spLauncher.nvim](https://github.com/speelbarrow/spLauncher.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2024-07-02 - For launching tasks, I guess.
* [mikeboiko/nvim-flow](https://github.com/mikeboiko/nvim-flow) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-07-28 - File-scoped command runner with YAML configuration, command preview, debug integration, and traceback quickfix.
* [sektant1/executioner.nvim](https://github.com/sektant1/executioner.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-05-03 - Script picker and runner to find and run any script from your project directory, with or without arguments.
* [niuiic/task.nvim](https://github.com/niuiic/task.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-02-26 - Another highly configurable task manager that enables seamless interaction with tasks.
* [wsdjeg/code-runner.nvim](https://github.com/wsdjeg/code-runner.nvim) ⭐ 6 | 🐛 1 | 🌐 Lua | 📅 2026-07-17 - Async code runner with range support.
* [negativo/nx-nvim](https://github.com/negativo/nx-nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-06-03 - Telescope picker for NX monorepo projects and targets, running the selected one in a split terminal.
* [JulOuellet/bzl.nvim](https://github.com/JulOuellet/bzl.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-08-02 - Bazel integration: target picker and tree, run/test/build with streaming output, and LSP support for Bazel-managed dependencies.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Neovim Lua Development

* [nvim-mini/mini.nvim#mini.doc](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-doc.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for generation of help files from EmmyLua-like annotations. Allows flexible customization of output via hook functions.
* [nvim-mini/mini.nvim#mini.test](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-test.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with framework for writing extensive plugin tests with support for hierarchical tests, hooks, parametrization, filtering, screen tests, "busted-style" emulation, customizable reporters, and more.
* [nvim-lua/plenary.nvim](https://github.com/nvim-lua/plenary.nvim) ⭐ 3,492 | 🐛 157 | 🌐 Lua | 📅 2026-04-10 - Plenary: full; complete; entire; absolute; unqualified. All the Lua functions I don't want to write twice.
* [MunifTanjim/nui.nvim](https://github.com/MunifTanjim/nui.nvim) ⭐ 2,106 | 🐛 24 | 🌐 Lua | 📅 2026-08-15 - UI Component Library.
* [folke/lazydev.nvim](https://github.com/folke/lazydev.nvim) ⭐ 1,565 | 🐛 7 | 🌐 Lua | 📅 2026-03-14 - Faster LuaLS setup.
* [kkharji/sqlite.lua](https://github.com/kkharji/sqlite.lua) ⭐ 572 | 🐛 21 | 🌐 Lua | 📅 2025-03-14 - SQLite/LuaJIT bindings.
* [jbyuki/one-small-step-for-vimkind](https://github.com/jbyuki/one-small-step-for-vimkind) ⭐ 547 | 🐛 7 | 🌐 Lua | 📅 2026-01-12 - An adapter for the built-in Lua language that allows debugging any Lua code running within an editor instance.
* [OXY2DEV/helpview.nvim](https://github.com/OXY2DEV/helpview.nvim) ⭐ 379 | 🐛 0 | 🌐 Lua | 📅 2026-07-08 - A hackable and fancy `vimdoc/help` file viewer.
* [svermeulen/vimpeccable](https://github.com/svermeulen/vimpeccable) ⭐ 348 | 🐛 9 | 🌐 Lua | 📅 2022-04-24 - Commands to help write your .vimrc in Lua or any Lua based language.
* [bfredl/nvim-luadev](https://github.com/bfredl/nvim-luadev) ⭐ 289 | 🐛 2 | 🌐 Lua | 📅 2023-03-13 - REPL/debug console Lua plugins. The `:Luadev` command will open an scratch window which will show output from executing Lua code.
* [lumen-oss/lz.n](https://github.com/lumen-oss/lz.n) ⭐ 289 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - A simple lazy loading library for plugins.
* [DrKJeff16/wezterm-types](https://github.com/DrKJeff16/wezterm-types) ⭐ 220 | 🐛 2 | 🌐 Lua | 📅 2026-08-06 - WezTerm config type annotations for LuaLS, including support for community plugins.
* [ray-x/guihua.lua](https://github.com/ray-x/guihua.lua) ⭐ 190 | 🐛 6 | 🌐 Lua | 📅 2026-07-03 - A Lua UI library. Includes a fzy search bar, list view and tree view modules.
* [CWood-sdf/banana.nvim](https://github.com/CWood-sdf/banana.nvim) ⭐ 157 | 🐛 2 | 🌐 Lua | 📅 2025-12-09 - HTML renderer for plugin UIs.
* [gregorias/coop.nvim](https://github.com/gregorias/coop.nvim) ⭐ 145 | 🐛 0 | 🌐 Lua | 📅 2026-05-12 - Structured concurrency with Lua coroutines.
* [tjdevries/vlog.nvim](https://github.com/tjdevries/vlog.nvim) ⭐ 143 | 🐛 5 | 🌐 Lua | 📅 2023-10-30 - Single file, no dependency, easy copy and paste log file to add to your Lua plugins.
* [jrop/morph.nvim](https://github.com/jrop/morph.nvim) ⭐ 136 | 🐛 0 | 🌐 Lua | 📅 2026-08-01 - A React-like renderer for building interactive buffers/TUIs.
* [BirdeeHub/lze](https://github.com/BirdeeHub/lze) ⭐ 131 | 🐛 1 | 🌐 Lua | 📅 2026-07-06 - A lazy-loading library for plugins.
* [milisims/nvim-luaref](https://github.com/milisims/nvim-luaref) ⭐ 127 | 🐛 3 | 🌐 Vim script | 📅 2024-07-10 - A reference for built-in Lua functions.
* [YaroSpace/lua-console.nvim](https://github.com/YaroSpace/lua-console.nvim) ⭐ 95 | 🐛 1 | 🌐 Lua | 📅 2025-11-24 - A handy scratch pad / REPL / debug console for built-in Lua development.
* [saghen/blink.lib](https://github.com/saghen/blink.lib) ⭐ 62 | 🐛 6 | 🌐 Lua | 📅 2026-08-08 - Generic utilities for all other `blink.*` plugins.
* [lumen-oss/luarocks-tag-release](https://github.com/lumen-oss/luarocks-tag-release) ⭐ 57 | 🐛 10 | 🌐 Lua | 📅 2026-08-16 - A GitHub action that publishes your plugins to LuaRocks.
* [anuvyklack/animation.nvim](https://github.com/anuvyklack/animation.nvim) ⭐ 47 | 🐛 0 | 🌐 Lua | 📅 2022-09-18 - Create animations.
* [svermeulen/nvim-lusc](https://github.com/svermeulen/nvim-lusc) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2024-02-23 - Adds support for Structured Async/Concurrency in Lua.
* [chrisgve/databox.nvim](https://github.com/chrisgve/databox.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-05-26 - Encrypted storage for Lua tables using [age](https://github.com/FiloSottile/age) ⭐ 23,228 | 🐛 32 | 🌐 Go | 📅 2026-03-20 or compatible encryption tools for cryptographic safety.
* [2KAbhishek/utils.nvim](https://github.com/2KAbhishek/utils.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-07-16 - Powerful utilities to speed up plugin development.
* [nfrid/treesitter-utils](https://github.com/nfrid/treesitter-utils) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2024-06-13 - Some useful Tree-sitter methods.
* [niuiic/omega.nvim](https://github.com/niuiic/omega.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-03-13 - Missing functions for Lua plugin development.
* [DrKJeff16/nvim-luaref](https://github.com/DrKJeff16/nvim-luaref) ⭐ 3 | 🐛 0 | 🌐 Vim Script | 📅 2026-06-09 - Forked from `milisims/nvim-luaref`, adds built-in Lua 5.1 help docs.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Fennel

* [Olical/conjure](https://github.com/Olical/conjure) ⭐ 2,132 | 🐛 90 | 🌐 Fennel | 📅 2026-07-24 - Interactive evaluation (Clojure, Fennel, Janet, Racket, Hy, MIT Scheme, Guile).
* [Olical/aniseed](https://github.com/Olical/aniseed) ⭐ 645 | 🐛 7 | 🌐 Fennel | 📅 2025-06-12 - Configure and extend your editor with Fennel.
* [rktjmp/hotpot.nvim](https://github.com/rktjmp/hotpot.nvim) ⭐ 400 | 🐛 0 | 🌐 Fennel | 📅 2026-07-29 - Seamless, transparent Fennel inside your editor.
* [Olical/nfnl](https://github.com/Olical/nfnl) ⭐ 359 | 🐛 8 | 🌐 Fennel | 📅 2026-08-14 - Streamlined successor to Aniseed, compiling Fennel to Lua on file write.
* [udayvir-singh/tangerine.nvim](https://github.com/udayvir-singh/tangerine.nvim) ⭐ 225 | 🐛 9 | 🌐 Fennel | 📅 2024-10-18 - Tangerine provides a painless way to add Fennel to your config.
* [udayvir-singh/hibiscus.nvim](https://github.com/udayvir-singh/hibiscus.nvim) ⭐ 106 | 🐛 3 | 🌐 Fennel | 📅 2024-07-21 - Highly opinionated macros to elegantly write your config.
* [aileot/nvim-thyme](https://github.com/aileot/nvim-thyme) ⭐ 41 | 🐛 3 | 🌐 Fennel | 📅 2025-11-04 - Zero-overhead Fennel JIT compiler with safety rollbacks and [parinfer-rust](https://github.com/eraserhd/parinfer-rust) ⭐ 627 | 🐛 35 | 🌐 Rust | 📅 2026-08-15 integration.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Dependency Management

* [Saecki/crates.nvim](https://github.com/Saecki/crates.nvim) ⭐ 1,116 | 🐛 11 | 🌐 Lua | 📅 2026-04-13 - Rust dependency management for `Cargo.toml`.
* [vuki656/package-info.nvim](https://github.com/vuki656/package-info.nvim) ⭐ 597 | 🐛 0 | 🌐 Lua | 📅 2026-08-14 - Display latest package version as virtual text in package.json.
* [piersolenski/import.nvim](https://github.com/piersolenski/import.nvim) ⭐ 265 | 🐛 0 | 🌐 Lua | 📅 2026-04-05 - Import modules faster based on what you've already imported in your project.
* [JesperLundberg/projektgunnar.nvim](https://github.com/JesperLundberg/projektgunnar.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2026-06-04 - C# dependency manager with support for handling references between projects and solution files.
* [Silletr/LazyDeveloperHelper](https://github.com/Silletr/LazyDeveloperHelper) ⭐ 18 | 🐛 0 | 🌐 Python | 📅 2026-07-05 - Python dependencies manager, with auto-adding to your `requirements.txt` file.
* [taigrr/glaze.nvim](https://github.com/taigrr/glaze.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Centralized manager for Go binaries, with parallel installs, auto-update checking, and a Mason-style UI.
* [DrKJeff16/pipenv.nvim](https://github.com/DrKJeff16/pipenv.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-07-08 - Asynchronous `Pipenv` manager with `spinner.nvim` integration.
* [cosmicbuffalo/gem\_install.nvim](https://github.com/cosmicbuffalo/gem_install.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-02-09 - Install Ruby gems, trigger `bundle install` and `gem install` with progress and caching to prevent retries when installs fail.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Git

* [nvim-mini/mini.nvim#mini.diff](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-diff.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to interactively visualize difference between buffer text and its reference. Provides toggleable detailed overview in text area, built-in apply/reset/textobject/goto mappings, and more.
* [nvim-mini/mini.nvim#mini.git](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-git.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for enhanced Git integration with current editor process that implements tracking of Git related data, `:Git` user command, and various helpers to explore Git history.
* [lewis6991/gitsigns.nvim](https://github.com/lewis6991/gitsigns.nvim) ⭐ 7,047 | 🐛 39 | 🌐 Lua | 📅 2026-08-11 - Git integration: signs, hunk actions, blame, etc.
* [NeogitOrg/neogit](https://github.com/NeogitOrg/neogit) ⭐ 5,586 | 🐛 197 | 🌐 Lua | 📅 2026-07-27 - A Magit clone that may change some things to fit the Vim philosophy.
* [kdheepak/lazygit.nvim](https://github.com/kdheepak/lazygit.nvim) ⭐ 2,339 | 🐛 53 | 🌐 Lua | 📅 2025-12-19 - Plugin for calling lazygit.
* [esmuellert/codediff.nvim](https://github.com/esmuellert/codediff.nvim) ⭐ 1,517 | 🐛 81 | 🌐 Lua | 📅 2026-08-11 - Side-by-side diff with two-tier highlighting (line + character level) using VSCode's algorithm implemented in C.
* [f-person/git-blame.nvim](https://github.com/f-person/git-blame.nvim) ⭐ 1,101 | 🐛 12 | 🌐 Lua | 📅 2025-11-05 - Show Git blame info.
* [tanvirtin/vgit.nvim](https://github.com/tanvirtin/vgit.nvim) ⭐ 850 | 🐛 17 | 🌐 Lua | 📅 2026-03-28 - Visual Git Plugin to enhance your Git experience.
* [SuperBo/fugit2.nvim](https://github.com/SuperBo/fugit2.nvim) ⭐ 474 | 🐛 16 | 🌐 Lua | 📅 2026-06-07 - Git GUI powered by [libgit2](https://libgit2.org).
* [harrisoncramer/GitLab.nvim](https://github.com/harrisoncramer/GitLab.nvim) ⭐ 397 | 🐛 19 | 🌐 Lua | 📅 2026-08-11 - Review pull requests and manage other GitLab resources.
* [aaronhallaert/advanced-git-search.nvim](https://github.com/aaronhallaert/advanced-git-search.nvim) ⭐ 391 | 🐛 4 | 🌐 Lua | 📅 2025-12-09 - Search your Git history by commit content, message and author with Telescope.
* [dlyongemallo/diffview.nvim](https://github.com/dlyongemallo/diffview.nvim) ⭐ 293 | 🐛 9 | 🌐 Lua | 📅 2026-08-16 - Single tabpage interface for easily cycling through diffs for all modified files for any Git rev. Maintained fork of sindrets/diffview\.nvim.
* [chojs23/ec](https://github.com/chojs23/ec) ⭐ 290 | 🐛 1 | 🌐 Go | 📅 2026-06-11 - A TUI native Git mergetool with 3 panes.
* [linrongbin16/gitlinker.nvim](https://github.com/linrongbin16/gitlinker.nvim) ⭐ 283 | 🐛 2 | 🌐 Lua | 📅 2026-06-07 - Maintained fork of "ruifm's gitlinker", refactored with bug fixes, ssh aliases, blame support and other improvements.
* [chrisgrieser/nvim-tinygit](https://github.com/chrisgrieser/nvim-tinygit) ⭐ 212 | 🐛 0 | 🌐 Lua | 📅 2026-08-12 - Lightweight and nimble Git client.
* [barrettruth/diffs.nvim](https://github.com/barrettruth/diffs.nvim) ⭐ 197 | 🐛 1 | 🌐 Lua | 📅 2026-08-15 - Syntax highlighting for diffs with Tree-sitter support for `vim-fugitive` and `&diff` buffers.
* [tveskag/nvim-blame-line](https://github.com/tveskag/nvim-blame-line) ⭐ 189 | 🐛 3 | 🌐 Vim Script | 📅 2026-03-18 - A small plugin that uses the virtual text to print Git blame info at the end of the current line.
* [axkirillov/unified.nvim](https://github.com/axkirillov/unified.nvim) ⭐ 141 | 🐛 1 | 🌐 Lua | 📅 2026-08-10 - Displaying inline unified diffs directly in your buffer.
* [kokusenz/deltaview.nvim](https://github.com/kokusenz/deltaview.nvim) ⭐ 126 | 🐛 6 | 🌐 Lua | 📅 2026-08-12 - Inline/unified diff viewer with Tree-sitter syntax highlighting and diff highlighting in the style of [delta](https://github.com/dandavison/delta) ⭐ 31,768 | 🐛 428 | 🌐 Rust | 📅 2026-08-02, with enhanced navigational features.
* [moyiz/git-dev.nvim](https://github.com/moyiz/git-dev.nvim) ⭐ 114 | 🐛 1 | 🌐 Lua | 📅 2026-04-13 - Open remote Git repositories while editing.
* [trevorhauter/gitportal.nvim](https://github.com/trevorhauter/gitportal.nvim) ⭐ 93 | 🐛 0 | 🌐 Lua | 📅 2025-12-21 - Generate Git permalinks, open them in your browser, load files locally from permalinks, and more.
* [isak102/telescope-git-file-history.nvim](https://github.com/isak102/telescope-git-file-history.nvim) ⭐ 91 | 🐛 2 | 🌐 Lua | 📅 2026-02-16 - Open/preview contents of the current file at a specific commit, without using `git checkout`.
* [jceb/jiejie.nvim](https://github.com/jceb/jiejie.nvim) ⭐ 80 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Frontend for Jujutsu in the style of `fugitive`.
* [spacedentist/resolve.nvim](https://github.com/spacedentist/resolve.nvim) ⭐ 64 | 🐛 8 | 🌐 Lua | 📅 2026-01-25 - Resolve merge conflicts with ease.
* [StackInTheWild/headhunter.nvim](https://github.com/StackInTheWild/headhunter.nvim) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2025-10-22 - Fast and simple utility to hunt and resolve merge conflicts.
* [2KAbhishek/co-author.nvim](https://github.com/2KAbhishek/co-author.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2025-10-16 - Quickly add co-authors to commits.
* [yus-works/csc.nvim](https://github.com/yus-works/csc.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2025-10-15 - Conventional commit scope completion that learns from Git history.
* [YouSame2/inlinediff-nvim](https://github.com/YouSame2/inlinediff-nvim) ⭐ 33 | 🐛 1 | 🌐 Lua | 📅 2026-02-11 - Provides a better inline Git diff view, meant to be used alongside your favorite Git plugin (e.g. `gitsigns`).
* [yutkat/git-rebase-auto-diff.nvim](https://github.com/yutkat/git-rebase-auto-diff.nvim) ⭐ 33 | 🐛 1 | 🌐 Lua | 📅 2025-07-19 - Show diff automatically when Git rebase.
* [AckslD/nvim-gfold.lua](https://github.com/AckslD/nvim-gfold.lua) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2022-10-19 - Plugin using [gfold](https://github.com/nickgerace/gfold) ⭐ 400 | 🐛 8 | 🌐 Rust | 📅 2026-06-10 to switch repo and have statusline component.
* [Salanoid/gitlogdiff.nvim](https://github.com/Salanoid/gitlogdiff.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-07-30 - Diff between multiple Git commits, similar to JetBrains's Git log.
* [9seconds/repolink.nvim](https://github.com/9seconds/repolink.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2023-12-08 - Generate shareable HTTP permalinks for various Git web frontends.
* [niuiic/git-log.nvim](https://github.com/niuiic/git-log.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-02-26 - Check Git log of the selected code.
* [Yu-Leo/blame-column.nvim](https://github.com/Yu-Leo/blame-column.nvim) ⭐ 20 | 🐛 5 | 🌐 Lua | 📅 2025-04-16 - Show Git blame info.
* [404pilo/aicommits.nvim](https://github.com/404pilo/aicommits.nvim) ⭐ 16 | 🐛 2 | 🌐 Lua | 📅 2026-08-01 - Generate conventional commit messages using AI.
* [mrloop/telescope-git-branch.nvim](https://github.com/mrloop/telescope-git-branch.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2024-07-08 - A telescope picker to find which files and preview what changes have been made to your Git branch across multiple commits.
* [Kohei-Wada/yadm-git.nvim](https://github.com/Kohei-Wada/yadm-git.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-06-23 - Seamless Git plugin support for yadm dotfiles.
* [wsdjeg/git.nvim](https://github.com/wsdjeg/git.nvim) ⭐ 12 | 🐛 1 | 🌐 Lua | 📅 2026-07-26 - An asynchronous Git command wrapper plugin, using `:Git` command instead of `:!git`.
* [Mauritz8/gitstatus.nvim](https://github.com/Mauritz8/gitstatus.nvim) ⭐ 12 | 🐛 6 | 🌐 Lua | 📅 2026-05-13 - Interactive Git status window with support for staging, unstaging, and committing files.
* [Sengoku11/commitpad.nvim](https://github.com/Sengoku11/commitpad.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-06-09 - Write informative commits with persistent worktree-isolated drafts, visual 50/72 guides, and a Markdown buffer.
* [Enigama/remarks.nvim](https://github.com/Enigama/remarks.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2026-01-17 - Personal developer notes attached to Git commits.
* [BibekBhusal0/nvim-git-utils](https://github.com/BibekBhusal0/nvim-git-utils) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-06-30 - Simple commands to make life easier while working with Git.
* [ajatdarojat45/commitmate.nvim](https://github.com/ajatdarojat45/commitmate.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-12-24 - An AI-assisted commit message generator following common commit conventions.

### GitHub

* [pwntester/octo.nvim](https://github.com/pwntester/octo.nvim) ⭐ 3,362 | 🐛 229 | 🌐 Lua | 📅 2026-07-30 - Work with GitHub issues and PRs.
* [ldelossa/gh.nvim](https://github.com/ldelossa/gh.nvim) ⭐ 651 | 🐛 34 | 🌐 Lua | 📅 2025-01-21 - A fully featured GitHub integration for performing code reviews.
* [rawnly/gist.nvim](https://github.com/rawnly/gist.nvim) ⭐ 217 | 🐛 0 | 🌐 Lua | 📅 2026-05-12 - Create a GitHub Gist from the current file (powered by gh).
* [justinmk/guh.nvim](https://github.com/justinmk/guh.nvim) ⭐ 209 | 🐛 23 | 🌐 Lua | 📅 2026-06-25 - View any GitHub object, including CI logs.
* [topaxi/pipeline.nvim](https://github.com/topaxi/pipeline.nvim) ⭐ 183 | 🐛 3 | 🌐 Lua | 📅 2026-07-22 - View and dispatch GitHub Actions workflow and GitLab CI pipeline runs.
* [2KAbhishek/octohub.nvim](https://github.com/2KAbhishek/octohub.nvim) ⭐ 79 | 🐛 0 | 🌐 Lua | 📅 2026-07-16 - Access all your gihub repos, stats and more in simple keystrokes.
* [gh-tui-tools/gh-review.nvim](https://github.com/gh-tui-tools/gh-review.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2026-08-04 - Review GitHub PRs.
* [claydugo/browsher.nvim](https://github.com/claydugo/browsher.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - Create commit pinned links to GitHub hosted files/lines.
* [3ZsForInsomnia/revman.nvim](https://github.com/3ZsForInsomnia/revman.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-04-21 - Track PRs that need review automatically and open them in Octo.nvim.
* [comatory/gh-co.nvim](https://github.com/comatory/gh-co.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2025-12-28 - Show the code owner(s) for files according to GitHub's `CODEOWNERS` specification.
* [mesirendon/nvim-ghrelease](https://github.com/mesirendon/nvim-ghrelease) ⭐ 6 | 🐛 1 | 🌐 Lua | 📅 2026-08-09 - Create a new GitHub release based on current releases of the repo.
* [cd-4/git-needy.nvim](https://github.com/cd-4/git-needy.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-03-08 - Keeps a tally of workflows that need to be reviewed in your statusbar.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Motion

* [nvim-mini/mini.nvim#mini.jump](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-jump.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for smarter jumping to a single character.
* [nvim-mini/mini.nvim#mini.jump2d](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-jump2d.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for smarter jumping within visible lines via iterative label filtering. Supports custom jump targets (spots), labels, hooks, allowed windows and lines, and more.
* [nvim-mini/mini.nvim#mini.bracketed](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-bracketed.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to go forward/backward with square brackets.
* [ggandor/leap.nvim](https://github.com/ggandor/leap.nvim) ⭐ 5,030 | 🐛 27 | 🌐 Fennel | 📅 2026-07-27 - A refined successor of Lightspeed, aiming to establish a widely accepted standard interface extension for moving around in Vim-like editors.
* [folke/flash.nvim](https://github.com/folke/flash.nvim) ⭐ 4,204 | 🐛 29 | 🌐 Lua | 📅 2026-07-10 - Navigate your code with search labels, enhanced character motions and Tree-sitter integration.
* [ggandor/lightspeed.nvim](https://github.com/ggandor/lightspeed.nvim) ⚠️ Archived - A Sneak-like plugin offering unparalleled navigation speed via ahead-of-time displayed labels, that eliminate the pause between entering the search pattern and selecting the target.
* [tris203/precognition.nvim](https://github.com/tris203/precognition.nvim) ⭐ 1,380 | 🐛 1 | 🌐 Lua | 📅 2026-07-26 - Precognition uses virtual text and gutter signs to show available motions.
* [chrisgrieser/nvim-spider](https://github.com/chrisgrieser/nvim-spider) ⭐ 898 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Use the w, e, b motions like a spider. Considers camelCase and skips insignificant punctuation.
* [abecodes/tabout.nvim](https://github.com/abecodes/tabout.nvim) ⭐ 861 | 🐛 7 | 🌐 Lua | 📅 2024-12-10 - Jump out of bracket pairs, quotes, objects, etc.
* [smoka7/hop.nvim](https://github.com/smoka7/hop.nvim) ⭐ 802 | 🐛 32 | 🌐 Lua | 📅 2026-08-14 - Hop is an EasyMotion-like plugin allowing you to jump anywhere in a document with as few keystrokes as possible.
* [Aaronik/Treewalker.nvim](https://github.com/aaronik/Treewalker.nvim) ⭐ 613 | 🐛 1 | 🌐 Lua | 📅 2026-07-31 - Move seamlessly around the abstract syntax tree.
* [ggandor/flit.nvim](https://github.com/ggandor/flit.nvim) ⭐ 411 | 🐛 18 | 🌐 Lua | 📅 2025-10-09 - Enhanced f/t motions for Leap.
* [rlane/pounce.nvim](https://github.com/rlane/pounce.nvim) ⭐ 366 | 🐛 7 | 🌐 Lua | 📅 2024-09-12 - An EasyMotion-like plugin for quick cursor movement using fuzzy search.
* [cbochs/portal.nvim](https://github.com/cbochs/portal.nvim) ⭐ 366 | 🐛 7 | 🌐 Lua | 📅 2024-06-03 - Build upon and enhance existing jumplist motions (i.e. `<c-i>` and `<c-o>`).
* [ggandor/leap-spooky.nvim](https://github.com/ggandor/leap-spooky.nvim) ⭐ 282 | 🐛 8 | 🌐 Lua | 📅 2024-02-08 - Spooky (Leap) actions at a distance.
* [woosaaahh/sj.nvim](https://github.com/woosaaahh/sj.nvim) ⭐ 130 | 🐛 0 | 🌐 Lua | 📅 2023-08-06 - Search based navigation combined with quick jump features.
* [liangxianzhe/nap.nvim](https://github.com/liangxianzhe/nap.nvim) ⭐ 103 | 🐛 1 | 🌐 Lua | 📅 2023-11-13 - Jump between next/previous buffer, tab, diagnostic, etc, with a single key.
* [rasulomaroff/telepath.nvim](https://github.com/rasulomaroff/telepath.nvim) ⭐ 71 | 🐛 1 | 🌐 Lua | 📅 2024-05-02 - Another Leap extension for performing remote actions with a different approach.
* [HawkinsT/pathfinder.nvim](https://github.com/HawkinsT/pathfinder.nvim) ⭐ 65 | 🐛 5 | 🌐 Lua | 📅 2025-11-17 - Enhances gf/gF/gx with look-ahead and smarter file, line/column number, and link resolution. Also provides visual targets for files/links, new motion commands, and link description retrieval.
* [backdround/neowords.nvim](https://github.com/backdround/neowords.nvim) ⭐ 63 | 🐛 2 | 🌐 Lua | 📅 2024-09-04 - Hops by any type of words. It gives fine control over `w`, `e`, `b`, `ge` movements.
* [kkew3/jieba.vim](https://github.com/kkew3/jieba.vim) ⭐ 60 | 🐛 1 | 🌐 Rust | 📅 2026-08-09 - Word motions and word text objects for Chinese.
* [backdround/improved-ft.nvim](https://github.com/backdround/improved-ft.nvim) ⭐ 45 | 🐛 1 | 🌐 Lua | 📅 2024-01-16 - Improve default `f`/`t` abilities.
* [kiyoon/repeatable-move.nvim](https://github.com/kiyoon/repeatable-move.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2026-04-01 - Make any motion repeatable with `;` and `,` keys.
* [nolleh/warp.nvim](https://github.com/nolleh/warp.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2026-07-13 - Jump based on labels to file paths, URLs, and Markdown links from any buffer.
* [xiaoshihou514/squirrel.nvim](https://github.com/xiaoshihou514/squirrel.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2024-01-04 - Quickly jump between Tree-sitter nodes.
* [timseriakov/spamguard.nvim](https://github.com/timseriakov/spamguard.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2025-05-05 - Detects excessive key spamming (jjjj/kkkk) and suggests more efficient alternatives.
* [Mr-LLLLL/treesitter-outer](https://github.com/Mr-LLLLL/treesitter-outer) ⭐ 10 | 🐛 1 | 🌐 Scheme | 📅 2024-06-10 - Jump to outer node with smart.
* [millerjason/neovimacs.nvim](https://github.com/millerjason/neovimacs.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - Provides Emacs movement and buffer keybindings while in insert mode.
* [cosmicbuffalo/eyeliner.nvim](https://github.com/cosmicbuffalo/eyeliner.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-06 - Highlight jump destinations for `f`/`t` motions.

### Tree-sitter Based

* [mfussenegger/nvim-treehopper](https://github.com/mfussenegger/nvim-treehopper) ⭐ 464 | 🐛 7 | 🌐 Lua | 📅 2025-06-16 - Region selection with hints on the AST nodes of a document powered by Tree-sitter.
* [drybalka/tree-climber.nvim](https://github.com/drybalka/tree-climber.nvim) ⭐ 159 | 🐛 0 | 🌐 Lua | 📅 2025-12-26 - Easy navigation around the Tree-sitter's tree that works in multi-language files and in normal mode.
* [kiyoon/treesitter-indent-object.nvim](https://github.com/kiyoon/treesitter-indent-object.nvim) ⭐ 74 | 🐛 2 | 🌐 Lua | 📅 2025-10-31 - Context-aware indent textobject powered by Tree-sitter.
* [atusy/treemonkey.nvim](https://github.com/atusy/treemonkey.nvim) ⭐ 41 | 🐛 1 | 🌐 Lua | 📅 2026-08-05 - Region selection with Tree-sitter nodes.
* [subev/sibling-jump.nvim](https://github.com/subev/sibling-jump.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-02-03 - Context-aware navigation between sibling Tree-sitter nodes.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Keybinding

* [nvim-mini/mini.nvim#mini.clue](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-clue.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to show next key clues. Has opt-in triggers, shows next key information after customizable delay, allows hydra-like submodes, and more.
* [nvim-mini/mini.nvim#mini.keymap](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-keymap.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with utilities to make special key mappings: multi-step actions (with built-in steps for "smart" `<Tab>`, `<S-Tab>`, `<CR>`, `<BS>`), combos (more general version of "better escape" like behavior).
* [folke/which-key.nvim](https://github.com/folke/which-key.nvim) ⭐ 7,260 | 🐛 39 | 🌐 Lua | 📅 2025-10-28 - Shows a popup with possible keybindings of the command you started typing.
* [mrjones2014/legendary.nvim](https://github.com/mrjones2014/legendary.nvim) ⚠️ Archived - Define your keymaps, commands, and autocommands as simple Lua tables, and create a legend for them at the same time (like VSCode's Command Palette), integrates with `which-key.nvim`.
* [max397574/better-escape.nvim](https://github.com/max397574/better-escape.nvim) ⭐ 795 | 🐛 3 | 🌐 Lua | 📅 2026-04-22 - Create shortcuts to escape insert mode without getting delay.
* [notomo/gesture.nvim](https://github.com/notomo/gesture.nvim) ⭐ 546 | 🐛 0 | 🌐 Lua | 📅 2026-08-16 - Mouse gesture plugin.
* [FeiyouG/commander.nvim](https://github.com/FeiyouG/commander.nvim) ⭐ 428 | 🐛 7 | 🌐 Lua | 📅 2024-06-08 - Create and manage keybindings and commands in a more organized manner and search them quickly through Telescope.
* [chrisgrieser/nvim-recorder](https://github.com/chrisgrieser/nvim-recorder) ⭐ 289 | 🐛 2 | 🌐 Lua | 📅 2026-08-03 - Simplifying and improving how you interact with macros.
* [nvimtools/hydra.nvim](https://github.com/nvimtools/hydra.nvim) ⭐ 281 | 🐛 10 | 🌐 Lua | 📅 2025-05-03 - Create custom submodes and menus. Port of Emacs Hydra. Maintained fork of anuvyklack/hydra.nvim.
* [tris203/hawtkeys.nvim](https://github.com/tris203/hawtkeys.nvim) ⭐ 252 | 🐛 8 | 🌐 Lua | 📅 2026-03-09 - Suggest new easy-to-hit keymaps and find issues with your current keymap configurations.
* [Wansmer/langmapper.nvim](https://github.com/Wansmer/langmapper.nvim) ⭐ 249 | 🐛 1 | 🌐 Lua | 📅 2026-03-24 - Auto translating your mappings for non-English input methods.
* [LionC/nest.nvim](https://github.com/LionC/nest.nvim) ⭐ 234 | 🐛 9 | 🌐 Lua | 📅 2022-10-28 - Lua utility to map keys concisely using cascading trees. Also allows binding Lua functions to keys.
* [mawkler/demicolon.nvim](https://github.com/mawkler/demicolon.nvim) ⭐ 133 | 🐛 0 | 🌐 Lua | 📅 2026-06-20 - Use `;` and `,` keys to also repeat jumps to diagnostics (e.g. `]d`) and to [nvim-treesitter-textobjects](https://github.com/nvim-treesitter/nvim-treesitter-textobjects?tab=readme-ov-file#text-objects-move) ⭐ 2,809 | 🐛 124 | 🌐 Tree-sitter Query | 📅 2026-07-19 (e.g. `]f`), in addition to repeating `t`/`T`/`f`/`F`.
* [zdcthomas/yop.nvim](https://github.com/zdcthomas/yop.nvim) ⭐ 87 | 🐛 3 | 🌐 Lua | 📅 2023-05-29 - Easily create your own operators (like `d` and `y`).
* [Nexmean/caskey.nvim](https://github.com/Nexmean/caskey.nvim) ⚠️ Archived - Utility to keymappings configuration using declarative cascading trees, optionally integrates with `which-key`.
* [kamegoro/tobira.nvim](https://github.com/kamegoro/tobira.nvim) ⭐ 54 | 🐛 13 | 🌐 Lua | 📅 2026-08-16 - Watches your keystrokes and suggests the one command you are missing, based on your actual usage patterns.
* [Iron-E/nvim-cartographer](https://github.com/Iron-E/nvim-cartographer) ⭐ 54 | 🐛 0 | 🌐 Lua | 📅 2023-06-19 - A more convenient `:map`ping syntax for Lua environments.
* [TheBlob42/houdini.nvim](https://github.com/TheBlob42/houdini.nvim) ⭐ 43 | 🐛 1 | 🌐 Lua | 📅 2024-07-05 - Create shortcut to escape modes without delay.
* [slugbyte/unruly-worker.nvim](https://github.com/slugbyte/unruly-worker.nvim) ⭐ 40 | 🐛 1 | 🌐 Lua | 📅 2025-12-22 - A ridiculously fun alternative keymap for the workman keyboard layout, with lots of powerful features for working with yank, marks, macros, LSP, and more. Built and configured with Lua.
* [RutaTang/compter.nvim](https://github.com/RutaTang/compter.nvim) ⭐ 29 | 🐛 1 | 🌐 Lua | 📅 2023-06-01 - Power and extend the ability of `<C-a>` and `<C-x>` with customized patterns.
* [sontungexpt/bim.nvim](https://github.com/sontungexpt/bim.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2026-06-11 - Enhances insert mode key mapping by showing typed keys in real time, without waiting for timeoutlen. It provides a responsive and intuitive insert-mode experience, ideal for complex input workflows like ime.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Scrolling

* [karb94/neoscroll.nvim](https://github.com/karb94/neoscroll.nvim) ⭐ 2,063 | 🐛 11 | 🌐 Lua | 📅 2025-12-31 - Smooth scrolling.
* [declancm/cinnamon.nvim](https://github.com/declancm/cinnamon.nvim) ⭐ 397 | 🐛 8 | 🌐 Lua | 📅 2024-08-07 - Smooth scrolling for any movement command.
* [saghen/filler-begone.nvim](https://github.com/saghen/filler-begone.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2025-10-30 - Prevents scrolling past the bottom of the buffer and showing unnecessary filler lines.
* [niuiic/scroll.nvim](https://github.com/niuiic/scroll.nvim) ⭐ 20 | 🐛 0 | 🌐 Lua | 📅 2024-05-24 - Smooth scrolling, custom smooth strategy.
* [rlychrisg/keepcursor.nvim](https://github.com/rlychrisg/keepcursor.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2024-08-23 - A collection of functions to control how the screen is positioned around the cursor.

### Scrollbar

* [nvim-mini/mini.nvim#mini.map](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-map.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to show floating window with buffer text overview, scrollbar, and highlights.
* [petertriho/nvim-scrollbar](https://github.com/petertriho/nvim-scrollbar) ⭐ 1,067 | 🐛 29 | 🌐 Lua | 📅 2026-08-16 - Extensible scrollbar that shows diagnostics and search results.
* [lewis6991/satellite.nvim](https://github.com/lewis6991/satellite.nvim) ⭐ 744 | 🐛 17 | 🌐 Lua | 📅 2026-05-01 - Decorate scrollbar.
* [dstein64/nvim-scrollview](https://github.com/dstein64/nvim-scrollview) ⭐ 699 | 🐛 4 | 🌐 Lua | 📅 2026-08-10 - Display interactive scrollbars.
* [gorbit99/codewindow.nvim](https://github.com/gorbit99/codewindow.nvim) ⭐ 485 | 🐛 26 | 🌐 Lua | 📅 2025-05-22 - Minimap plugin, that is closely integrated with Tree-sitter and the built-in LSP to display more information to the user.
* [Xuyuanp/scrollbar.nvim](https://github.com/Xuyuanp/scrollbar.nvim) ⭐ 286 | 🐛 9 | 🌐 Lua | 📅 2025-03-23 - Scrollbar.
* [wsdjeg/scrollbar.nvim](https://github.com/wsdjeg/scrollbar.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2026-07-18 - Floating scrollbar.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Editing Support

* [nvim-mini/mini.nvim#mini.pairs](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-pairs.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for autopairs which has minimal defaults and functionality to do per-key mapping.
* [nvim-mini/mini.nvim#mini.trailspace](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-trailspace.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for automatic highlighting of trailing whitespace with functionality to remove it.
* [nvim-mini/mini.nvim#mini.operators](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-operators.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with various text edit operators: replace, exchange, multiply, sort, evaluate.
* [nvim-mini/mini.nvim#mini.move](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-move.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to move any selection (charwise, linewise, blockwise, current line in Normal mode) in any direction. Handles both `v:count` and undo history.
* [nvim-mini/mini.nvim#mini.ai](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-ai.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for extending and creating `a`/`i` textobjects. It enhances some built-in textobjects, creates extensive set of new ones (like `a*`, `a<Space>`, `a?`, and more), and allows user to create their own (via Lua patterns or functions). Supports dot-repeat, different search methods, consecutive application, and more.
* [nvim-mini/mini.nvim#mini.splitjoin](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-splitjoin.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to split and join arguments. Has customizable pre and post hooks. Works inside comments.
* [nvim-mini/mini.nvim#mini.basics](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-basics.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` with customizable configuration presets for common options, mappings, and autocommands.
* [windwp/nvim-autopairs](https://github.com/windwp/nvim-autopairs) ⭐ 4,080 | 🐛 18 | 🌐 Lua | 📅 2026-05-08 - A minimalist autopairs written by Lua.
* [nvim-treesitter/nvim-treesitter-context](https://github.com/nvim-treesitter/nvim-treesitter-context) ⭐ 3,226 | 🐛 30 | 🌐 Janet | 📅 2026-08-02 - Shows floating hover with the current function/block context.
* [folke/zen-mode.nvim](https://github.com/folke/zen-mode.nvim) ⭐ 2,155 | 🐛 18 | 🌐 Lua | 📅 2025-10-28 - Distraction-free coding.
* [windwp/nvim-ts-autotag](https://github.com/windwp/nvim-ts-autotag) ⭐ 2,109 | 🐛 6 | 🌐 Lua | 📅 2026-04-15 - Use Tree-sitter to autoclose and autorename XML, HTML, JSX tag.
* [jake-stewart/multicursor.nvim](https://github.com/jake-stewart/multicursor.nvim) ⭐ 1,513 | 🐛 0 | 🌐 Lua | 📅 2026-03-24 - Adds support for multiple cursors which work how you expect.
* [Wansmer/treesj](https://github.com/Wansmer/treesj) ⭐ 1,339 | 🐛 9 | 🌐 Lua | 📅 2026-05-28 - Splitting/joining blocks of code like arrays, hashes, statements, objects, dictionaries, etc. Using Tree-sitter. Inspired by greatest splitjoin.vim.
* [gbprod/yanky.nvim](https://github.com/gbprod/yanky.nvim) ⭐ 1,283 | 🐛 34 | 🌐 Lua | 📅 2026-07-22 - Improved Yank and Put functionalities.
* [monaqa/dial.nvim](https://github.com/monaqa/dial.nvim) ⭐ 1,102 | 🐛 19 | 🌐 Lua | 📅 2025-12-21 - Extended increment/decrement.
* [cshuaimin/ssr.nvim](https://github.com/cshuaimin/ssr.nvim) ⭐ 1,010 | 🐛 18 | 🌐 Lua | 📅 2026-04-06 - Tree-sitter based structural search and replace.
* [shortcuts/no-neck-pain.nvim](https://github.com/shortcuts/no-neck-pain.nvim) ⭐ 963 | 🐛 16 | 🌐 Lua | 📅 2026-07-07 - Center the currently focused buffer to the middle of your terminal.
* [HiPhish/rainbow-delimiters.nvim](https://github.com/HiPhish/rainbow-delimiters.nvim) ⭐ 884 | 🐛 22 | 🌐 Lua | 📅 2026-07-29 - Rainbow delimiters with Tree-sitter.
* [nacro90/numb.nvim](https://github.com/nacro90/numb.nvim) ⭐ 868 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Peek lines in a non-obtrusive way.
* [debugloop/telescope-undo.nvim](https://github.com/debugloop/telescope-undo.nvim) ⭐ 790 | 🐛 6 | 🌐 Lua | 📅 2025-01-31 - A telescope extension to visualize your undo tree and fuzzy-search changes in it.
* [chrisgrieser/nvim-various-textobjs](https://github.com/chrisgrieser/nvim-various-textobjs) ⭐ 771 | 🐛 0 | 🌐 Lua | 📅 2026-08-03 - Bundle of more than 30 new text objects.
* [gbprod/substitute.nvim](https://github.com/gbprod/substitute.nvim) ⭐ 740 | 🐛 7 | 🌐 Lua | 📅 2026-02-17 - New operator motions to quickly replace and exchange text.
* [m4xshen/autoclose.nvim](https://github.com/m4xshen/autoclose.nvim) ⭐ 649 | 🐛 13 | 🌐 Lua | 📅 2026-07-20 - A minimalist autoclose plugin written in Lua.
* [smoka7/multicursors.nvim](https://github.com/smoka7/multicursors.nvim) ⭐ 643 | 🐛 13 | 🌐 Lua | 📅 2025-02-26 - Provides a more intuitive way to edit repetitive text with multiple selections.
* [altermo/ultimate-autopair.nvim](https://github.com/altermo/ultimate-autopair.nvim) ⭐ 579 | 🐛 22 | 🌐 Lua | 📅 2026-07-18 - Autopair with extensions.
* [smjonas/live-command.nvim](https://github.com/smjonas/live-command.nvim) ⭐ 538 | 🐛 10 | 🌐 Lua | 📅 2025-12-19 - Text editing with immediate visual feedback: preview commands such as `:norm`, `:g`, macros and more.
* [mizlan/iswap.nvim](https://github.com/mizlan/iswap.nvim) ⭐ 525 | 🐛 10 | 🌐 Lua | 📅 2026-05-29 - Interactively select and swap function arguments, list elements, and more. Powered by Tree-sitter.
* [brenton-leighton/multiple-cursors.nvim](https://github.com/brenton-leighton/multiple-cursors.nvim) ⭐ 422 | 🐛 1 | 🌐 Lua | 📅 2026-05-10 - A multi-cursor plugin that works in normal, insert/replace, or visual modes, and with almost every command.
* [andersevenrud/nvim\_context\_vt](https://github.com/andersevenrud/nvim_context_vt) ⭐ 415 | 🐛 3 | 🌐 Lua | 📅 2026-08-03 - Shows virtual text of the current context.
* [ckolkey/ts-node-action](https://github.com/CKolkey/ts-node-action) ⭐ 379 | 🐛 16 | 🌐 Lua | 📅 2026-01-16 - A framework for executing functional transformations on Tree-sitter nodes.
* [keaising/im-select.nvim](https://github.com/keaising/im-select.nvim) ⭐ 358 | 🐛 9 | 🌐 Lua | 📅 2026-03-18 - Switching and restoring input method automatically depending on the edit mode.
* [zbirenbaum/neodim](https://github.com/zbirenbaum/neodim) ⭐ 346 | 🐛 5 | 🌐 Lua | 📅 2025-01-09 - Dimming the highlights of unused functions, variables, parameters, and more.
* [okuuva/auto-save.nvim](https://github.com/okuuva/auto-save.nvim) ⭐ 328 | 🐛 3 | 🌐 Lua | 📅 2026-04-16 - Automatically saves your work as often as needed and as seldom as possible. Customizable with smart defaults. Maintained fork of Pocco81/auto-save.nvim.
* [filipdutescu/renamer.nvim](https://github.com/filipdutescu/renamer.nvim) ⭐ 318 | 🐛 10 | 🌐 Lua | 📅 2024-01-04 - VSCode-like renaming UI, written in Lua.
* [tomiis4/hypersonic.nvim](https://github.com/tomiis4/hypersonic.nvim) ⭐ 232 | 🐛 3 | 🌐 Lua | 📅 2024-08-11 - Provides explanation for RegExp.
* [gbprod/cutlass.nvim](https://github.com/gbprod/cutlass.nvim) ⭐ 231 | 🐛 2 | 🌐 Lua | 📅 2025-10-23 - Plugin that adds a 'cut' operation separate from 'delete'.
* [sQVe/sort.nvim](https://github.com/sQVe/sort.nvim) ⭐ 215 | 🐛 0 | 🌐 Lua | 📅 2026-04-17 - Sorting plugin that intelligently supports line-wise and delimiter sorting.
* [booperlv/nvim-gomove](https://github.com/booperlv/nvim-gomove) ⭐ 204 | 🐛 4 | 🌐 Lua | 📅 2022-07-19 - A complete plugin for moving and duplicating blocks and lines, with complete fold handling, reindenting, and undoing in one go.
* [nguyenvukhang/nvim-toggler](https://github.com/nguyenvukhang/nvim-toggler) ⭐ 201 | 🐛 3 | 🌐 Lua | 📅 2026-03-20 - Invert text, such as toggling between `true` and `false`.
* [nat-418/boole.nvim](https://github.com/nat-418/boole.nvim) ⭐ 189 | 🐛 12 | 🌐 Lua | 📅 2024-06-06 - Toggle booleans and common string values.
* [XXiaoA/atone.nvim](https://github.com/XXiaoA/atone.nvim) ⭐ 187 | 🐛 0 | 🌐 Lua | 📅 2026-08-15 - Undo tree for visualizing and managing undo history.
* [Wansmer/sibling-swap.nvim](https://github.com/Wansmer/sibling-swap.nvim) ⭐ 183 | 🐛 3 | 🌐 Lua | 📅 2026-04-06 - Different way to swapping arguments and other siblings with Tree-sitter.
* [gregorias/coerce.nvim](https://github.com/gregorias/coerce.nvim) ⭐ 174 | 🐛 0 | 🌐 Lua | 📅 2026-06-02 - Change keyword case.
* [AckslD/nvim-trevJ.lua](https://github.com/AckslD/nvim-trevJ.lua) ⭐ 171 | 🐛 6 | 🌐 Lua | 📅 2025-07-21 - Does the opposite of join-line (J) for arguments, powered by Tree-sitter.
* [nemanjamalesija/smart-paste.nvim](https://github.com/nemanjamalesija/smart-paste.nvim) ⭐ 170 | 🐛 1 | 🌐 Lua | 📅 2026-08-10 - Automatic indentation of pasted code using a three-tier indent strategy (indentexpr / Tree-sitter / heuristic).
* [willothy/moveline.nvim](https://github.com/willothy/moveline.nvim) ⭐ 153 | 🐛 6 | 🌐 Rust | 📅 2025-09-22 - Move lines and blocks up and down easily, with indenting handled automatically as you move. Written in Rust.
* [ZhiyuanLck/smart-pairs](https://github.com/ZhiyuanLck/smart-pairs) ⭐ 137 | 🐛 7 | 🌐 Lua | 📅 2025-11-23 - Ultimate smart pairs written by Lua.
* [OXY2DEV/foldtext.nvim](https://github.com/OXY2DEV/foldtext.nvim) ⭐ 130 | 🐛 2 | 🌐 Lua | 📅 2026-05-28 - Dynamic and stylized foldtext.
* [SunnyTamang/select-undo.nvim](https://github.com/SunnyTamang/select-undo.nvim) ⭐ 127 | 🐛 0 | 🌐 Lua | 📅 2026-07-05 - Allow users to undo specific line/lines or partial selections without affecting the rest of the file.
* [ptdewey/yankbank-nvim](https://github.com/ptdewey/yankbank-nvim) ⭐ 124 | 🐛 0 | 🌐 Lua | 📅 2026-04-19 - Enable streamlined access to recent yanks and deletions in a quick-access popup menu.
* [h-hg/fcitx.nvim](https://github.com/h-hg/fcitx.nvim) ⭐ 105 | 🐛 3 | 🌐 Lua | 📅 2025-12-28 - Switching and restoring fcitx state for each buffer separately.
* [gbprod/stay-in-place.nvim](https://github.com/gbprod/stay-in-place.nvim) ⭐ 99 | 🐛 1 | 🌐 Lua | 📅 2023-01-23 - Prevent the cursor from moving when using shift and filter actions.
* [bennypowers/splitjoin.nvim](https://github.com/bennypowers/splitjoin.nvim) ⭐ 99 | 🐛 0 | 🌐 Lua | 📅 2026-07-15 - Split and join various syntax structures.
* [tummetott/unimpaired.nvim](https://github.com/tummetott/unimpaired.nvim) ⚠️ Archived - Lua port of [tpope/vim-unimpaired](https://github.com/tpope/vim-unimpaired) ⭐ 3,464 | 🐛 56 | 🌐 Vim Script | 📅 2025-08-16.
* [chrisgrieser/nvim-puppeteer](https://github.com/chrisgrieser/nvim-puppeteer) ⭐ 77 | 🐛 1 | 🌐 Lua | 📅 2026-08-03 - Automatically convert strings to f-strings or template strings and back.
* [Jxstxs/conceal.nvim](https://github.com/Jxstxs/conceal.nvim) ⭐ 77 | 🐛 1 | 🌐 Lua | 📅 2024-07-07 - Use Tree-sitter to conceal common boilerplate code.
* [necrom4/convy.nvim](https://github.com/necrom4/convy.nvim) ⭐ 52 | 🐛 0 | 🌐 Lua | 📅 2026-06-07 - Easily convert strings between various formats.
* [kiyoon/telescope-insert-path.nvim](https://github.com/kiyoon/telescope-insert-path.nvim) ⭐ 46 | 🐛 1 | 🌐 Lua | 📅 2025-12-20 - Insert file path in the current buffer using Telescope.
* [attilarepka/header.nvim](https://github.com/attilarepka/header.nvim) ⭐ 45 | 🐛 0 | 🌐 Lua | 📅 2026-07-24 - Add or update copyright and license headers in any source file.
* [wurli/split.nvim](https://github.com/wurli/split.nvim) ⭐ 38 | 🐛 1 | 🌐 Lua | 📅 2025-02-07 - Provides a mapping to split text by delimiter, giving an inverse of the native J command.
* [XXiaoA/ns-textobject.nvim](https://github.com/XXiaoA/ns-textobject.nvim) ⭐ 37 | 🐛 4 | 🌐 Lua | 📅 2023-05-26 - Awesome textobject plugin works with nvim-surround.
* [altermo/iedit.nvim](https://github.com/altermo/iedit.nvim) ⭐ 36 | 🐛 0 | 🌐 Lua | 📅 2026-01-07 - Edit one occurrence of text and simultaneously have other selected occurrences edited in the same way.
* [Allendang/nvim-expand-expr](https://github.com/AllenDang/nvim-expand-expr) ⭐ 35 | 🐛 0 | 🌐 Lua | 📅 2021-08-14 - Expand and repeat expression to multiple lines.
* [zhisme/copy\_with\_context.nvim](https://github.com/zhisme/copy_with_context.nvim) ⭐ 35 | 🐛 12 | 🌐 Lua | 📅 2026-07-16 - Copy lines with file path and line number metadata for sharing code snippets with context.
* [qwavies/smart-backspace.nvim](https://github.com/qwavies/smart-backspace.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2026-07-17 - Context-aware backspace which handles pairs, whitespace and indentation.
* [csessh/stopinsert.nvim](https://github.com/csessh/stopinsert.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2026-08-11 - Automatically exit Insert mode after inactivity.
* [niuiic/divider.nvim](https://github.com/niuiic/divider.nvim) ⭐ 30 | 🐛 0 | 🌐 Lua | 📅 2024-11-18 - Custom code divider line.
* [nxhung2304/lastplace.nvim](https://github.com/nxhung2304/lastplace.nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - Intelligently restore your cursor position when reopening files.
* [hinell/duplicate.nvim](https://github.com/hinell/duplicate.nvim) ⭐ 25 | 🐛 0 | 🌐 Lua | 📅 2023-10-23 - Duplicate lines and blocks of lines easily; undo and unfolding support; full OOP.
* [rlychrisg/truncateline.nvim](https://github.com/rlychrisg/truncateline.nvim) ⭐ 22 | 🐛 0 | 🌐 Lua | 📅 2026-01-14 - Truncate long lines to keep track of where you are when the start gets lost off the left side of the screen.
* [tmillr/sos.nvim](https://github.com/tmillr/sos.nvim) ⭐ 22 | 🐛 12 | 🌐 Lua | 📅 2024-12-07 - Automatically save all your modified buffers according to a predefined timeout value.
* [daltongd/yanklock.nvim](https://github.com/daltongd/yanklock.nvim) ⭐ 21 | 🐛 0 | 🌐 Lua | 📅 2025-01-03 - Temporarily lock the paste register to `"0`, and use `d`, `c`, and `s` motions while keeping the most recent yanked content easily accessible.
* [Wansmer/binary-swap.nvim](https://github.com/Wansmer/binary-swap.nvim) ⚠️ Archived - Swapping operands and operators in binary expressions: comparison and mathematical operations.
* [tigion/swap.nvim](https://github.com/tigion/swap.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2025-10-08 - Quickly switch a word under the cursor or a pattern in the current line.
* [saifulapm/commasemi.nvim](https://github.com/saifulapm/commasemi.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2025-03-06 - Toggle comma and semicolon.
* [niuiic/part-edit.nvim](https://github.com/niuiic/part-edit.nvim) ⭐ 15 | 🐛 0 | 🌐 Lua | 📅 2026-01-16 - Edit a part of a file individually.
* [hinell/move.nvim](https://github.com/hinell/move.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2023-10-25 - Move chunks of text around; fork of [fedepujol/move.nvim](https://github.com/fedepujol/move.nvim) ⭐ 369 | 🐛 8 | 🌐 Lua | 📅 2025-05-13.
* [ntk148v/yankdown.nvim](https://github.com/ntk148v/yankdown.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-07-14 - Paste rich clipboard content as clean Markdown.
* [zongben/capsoff.nvim](https://github.com/zongben/capsoff.nvim) ⭐ 13 | 🐛 0 | 🌐 Lua | 📅 2024-12-27 - Turns off CapsLock when you leaving insert mode.
* [yaocccc/visual-multi.nvim](https://github.com/yaocccc/visual-multi.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-07-23 - A fast, core-focused multi-cursor plugin written in Lua with Normal, Insert, and Extend modes.
* [DRoma82/add-subtract-ex.nvim](https://github.com/DRoma82/add-subtract-ex.nvim) ⭐ 11 | 🐛 1 | 🌐 Lua | 📅 2026-08-14 - Extends `<C-a>`/`<C-x>` to toggle booleans, comparison/logical operators, and shift letters, deferring to native number handling.
* [DrKJeff16/boolean-toggle.nvim](https://github.com/DrKJeff16/boolean-toggle.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-07-04 - Toggle between `true` and `false` under your cursor.
* [DrKJeff16/shebang.nvim](https://github.com/DrKJeff16/shebang.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-08-09 - Add or modify a shebang on top of the current file.
* [kobbikobb/move-lines.nvim](https://github.com/kobbikobb/move-lines.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2025-01-01 - Moves lines selected in virtual mode.
* [neur1n/hyphen.nvim](https://github.com/neur1n/hyphen.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-06-15 - Show TeX-style hyphenation breakpoints in text.
* [hiberabyss/bzlops.vim](https://github.com/hiberabyss/bzlops.vim) ⭐ 4 | 🐛 0 | 🌐 Vim Script | 📅 2023-12-21 - Help to manage your bazel build rule.
* [Chiarandini/smart-enter.nvim](https://github.com/Chiarandini/smart-enter.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-08-07 - Context-aware newline that continues LaTeX environments, Markdown lists, and more.
* [TheLazyCat00/replace-nvim](https://github.com/TheLazyCat00/replace-nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2025-05-07 - Replace part of your code with the contents of the `+` register using textobjects.
* [\~nedia/auto-save.nvim](https://git.sr.ht/~nedia/auto-save.nvim) - Extremely simple auto saving on `InsertLeave` and `TextChanged`. Based on Pocco81/AutoSave but lighter.

### Comment

* [nvim-mini/mini.nvim#mini.comment](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-comment.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for per-line commenting. Fully supports dot-repeat.
* [numToStr/Comment.nvim](https://github.com/numToStr/Comment.nvim) ⭐ 4,666 | 🐛 83 | 🌐 Lua | 📅 2024-08-19 - Smart and powerful comment plugin. Supports commentstring, motions, dot-repeat and more.
* [folke/todo-comments.nvim](https://github.com/folke/todo-comments.nvim) ⭐ 4,199 | 🐛 24 | 🌐 Lua | 📅 2025-11-10 - Highlight, list and search TODO comments in your projects.
* [danymat/neogen](https://github.com/danymat/neogen) ⭐ 1,659 | 🐛 44 | 🌐 Lua | 📅 2026-01-10 - A better annotation generator which supports multiple languages and annotation conventions.
* [JoosepAlviste/nvim-ts-context-commentstring](https://github.com/JoosepAlviste/nvim-ts-context-commentstring) ⭐ 1,303 | 🐛 23 | 🌐 Lua | 📅 2026-04-04 - Sets the `commentstring` option based on the cursor location in the file. The location is checked via Tree-sitter queries.
* [b3nj5m1n/kommentary](https://github.com/b3nj5m1n/kommentary) ⭐ 532 | 🐛 8 | 🌐 Lua | 📅 2023-11-29 - Commenting plugin written in Lua.
* [LudoPinelli/comment-box.nvim](https://github.com/LudoPinelli/comment-box.nvim) ⭐ 501 | 🐛 17 | 🌐 Lua | 📅 2024-08-10 - Clarify and beautify your comments using boxes and lines.
* [terrortylor/nvim-comment](https://github.com/terrortylor/nvim-comment) ⭐ 497 | 🐛 14 | 🌐 Lua | 📅 2024-05-29 - Toggle comments using the built-in commentstring option.
* [winston0410/commented.nvim](https://github.com/winston0410/commented.nvim) ⭐ 114 | 🐛 4 | 🌐 Lua | 📅 2022-03-12 - A commenting plugin which supports counts and multiple comment patterns and much more.
* [jeangiraldoo/codedocs.nvim](https://github.com/jeangiraldoo/codedocs.nvim) ⭐ 109 | 🐛 1 | 🌐 Lua | 📅 2026-07-14 - A powerful and customizable annotation framework with support for many languages and annotation conventions.
* [s1n7ax/nvim-comment-frame](https://github.com/s1n7ax/nvim-comment-frame) ⭐ 101 | 🐛 1 | 🌐 Lua | 📅 2025-08-05 - Adds a comment frame based on the source file.
* [Zeioth/dooku.nvim](https://github.com/Zeioth/dooku.nvim) ⭐ 51 | 🐛 0 | 🌐 Lua | 📅 2025-06-24 - Generate and open your HTML code documentation.
* [gennaro-tedesco/nvim-commaround](https://github.com/gennaro-tedesco/nvim-commaround) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2023-01-06 - Fast and light commenting plugin written in Lua.
* [kuri-sun/todoage.nvim](https://github.com/kuri-sun/todoage.nvim) ⭐ 29 | 🐛 0 | 🌐 Lua | 📅 2026-06-28 - Show how old your TODOs are.
* [celeste3z/celeste\_comment.nvim](https://github.com/celeste3z/celeste_comment.nvim) ⭐ 27 | 🐛 0 | 🌐 Lua | 📅 2026-08-15 - VSCode-style commenting plugin with support for line and block comments, and textobjects.
* [georgeharker/comment-tasks.nvim](https://github.com/georgeharker/comment-tasks.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2026-06-12 - Keep your task manager up to date from TODO and FIXME comments in code.
* [alexmozaidze/tree-comment.nvim](https://github.com/alexmozaidze/tree-comment.nvim) ⭐ 13 | 🐛 1 | 🌐 Fennel | 📅 2025-11-19 - Highlight and configure TODO comments for [tree-sitter-comment](https://github.com/stsewd/tree-sitter-comment) ⭐ 169 | 🐛 11 | 🌐 C | 📅 2025-12-16.
* [LucasTavaresA/SingleComment.nvim](https://github.com/LucasTavaresA/SingleComment.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2025-08-27 - Always single line, comment sensitive, indentation preserving commenting.

### Folding

* [kevinhwang91/nvim-ufo](https://github.com/kevinhwang91/nvim-ufo) ⭐ 2,948 | 🐛 47 | 🌐 Lua | 📅 2026-01-11 - Ultra fold with modern looking and performance boosting.
* [chrisgrieser/nvim-origami](https://github.com/chrisgrieser/nvim-origami) ⭐ 526 | 🐛 4 | 🌐 Lua | 📅 2026-08-03 - Fold with relentless elegance.
* [jghauser/fold-cycle.nvim](https://github.com/jghauser/fold-cycle.nvim) ⭐ 92 | 🐛 0 | 🌐 Lua | 📅 2025-08-31 - Cycle folds open or closed.
* [malbertzard/inline-fold.nvim](https://github.com/malbertzard/inline-fold.nvim) ⭐ 89 | 🐛 4 | 🌐 Lua | 📅 2023-08-12 - Hide certain elements inline like long CSS classes or `href` content.
* [soemre/commentless.nvim](https://github.com/soemre/commentless.nvim) ⭐ 45 | 🐛 1 | 🌐 Lua | 📅 2025-04-26 - Fold all comments to better visualize your code logic, and unfold them whenever needed.
* [yaocccc/nvim-foldsign](https://github.com/yaocccc/nvim-foldsign) ⭐ 41 | 🐛 0 | 🌐 Lua | 📅 2025-03-18 - Display folds on sign column.
* [fold-logging.nvim](https://github.com/markosnarinian/fold-logging.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2026-06-22 - Fold logging/debug prints without changing normal folds.
* [netmute/foldsigns.nvim](https://github.com/netmute/foldsigns.nvim) ⭐ 6 | 🐛 0 | 🌐 Lua | 📅 2026-01-19 - Adds fold markers to sign column to make folds more visible while editing.
* [netmute/foldchanged.nvim](https://github.com/netmute/foldchanged.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-01-19 - Adds a `FoldChanged` User event.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Formatting

* [nvim-mini/mini.nvim#mini.align](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-align.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for aligning text interactively (with or without instant preview).
* [stevearc/conform.nvim](https://github.com/stevearc/conform.nvim) ⭐ 5,305 | 🐛 96 | 🌐 Lua | 📅 2026-08-11 - A lightweight formatting engine that plays nice with LSP.
* [sbdchd/neoformat](https://github.com/sbdchd/neoformat) ⭐ 2,048 | 🐛 130 | 🌐 Vim Script | 📅 2026-04-13 - A code formatting runner.
* [mhartington/formatter.nvim](https://github.com/mhartington/formatter.nvim) ⭐ 1,456 | 🐛 44 | 🌐 Lua | 📅 2025-05-29 - A format runner written in Lua.
* [nvimdev/guard.nvim](https://github.com/nvimdev/guard.nvim) ⭐ 520 | 🐛 0 | 🌐 Lua | 📅 2026-01-31 - Minimalist async formatting and linting plugin.
* [MunifTanjim/prettier.nvim](https://github.com/MunifTanjim/prettier.nvim) ⭐ 316 | 🐛 5 | 🌐 Lua | 📅 2025-04-08 - Prettier integration.
* [elentok/format-on-save.nvim](https://github.com/elentok/format-on-save.nvim) ⭐ 172 | 🐛 6 | 🌐 Lua | 📅 2025-07-20 - A synchronous formatter that combines both LSP and non-LSP formatting (e.g. `shfmt`, `stylua`, `prettier`). Focused specifically for format-on-save.
* [cappyzawa/trim.nvim](https://github.com/cappyzawa/trim.nvim) ⭐ 157 | 🐛 3 | 🌐 Lua | 📅 2026-06-18 - Trims trailing whitespace and lines.
* [emileferreira/nvim-strict](https://github.com/emileferreira/nvim-strict) ⭐ 41 | 🐛 0 | 🌐 Lua | 📅 2026-07-16 - Strict, native code style formatting which exposes deep nesting, overlong lines, trailing whitespace, trailing empty lines, TODOs and inconsistent indentation.
* [niuiic/format.nvim](https://github.com/niuiic/format.nvim) ⭐ 33 | 🐛 0 | 🌐 Lua | 📅 2025-08-02 - An asynchronous, multitasking, highly configurable formatting plugin.
* [tenxsoydev/tabs-vs-spaces.nvim](https://github.com/tenxsoydev/tabs-vs-spaces.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2024-09-22 - Hint and fix deviating indentation.
* [wsdjeg/format.nvim](https://github.com/wsdjeg/format.nvim) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2026-07-26 - An asynchronous code formatting plugin.
* [paul-louyot/toggle-quotes.nvim](https://github.com/paul-louyot/toggle-quotes.nvim) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2024-11-29 - Toggle between quotes.
* [TheLazyCat00/simple-format](https://github.com/TheLazyCat00/simple-format) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-04-03 - Replace text using custom regex and highlight group rules.
* [bennypowers/svgo.nvim](https://github.com/bennypowers/svgo.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-04-01 - Optimize SVG files.
* [\~nedia/auto-format.nvim](https://git.sr.ht/~nedia/auto-format.nvim) - Sets up an autocommand to format on save, preferring `null-ls` over native LSP client formatting.

### Indent

* [nvim-mini/mini.nvim#mini.indentscope](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-indentscope.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for visualizing and operating on indent scope. Supports customization of debounce delay, animation style, and different granularity of options for scope computing algorithm.
* [lukas-reineke/indent-blankline.nvim](https://github.com/lukas-reineke/indent-blankline.nvim) ⭐ 4,996 | 🐛 27 | 🌐 Lua | 📅 2026-02-17 - IndentLine replacement in Lua with more features and Tree-sitter support.
* [shellRaining/hlchunk.nvim](https://github.com/shellRaining/hlchunk.nvim) ⭐ 917 | 🐛 36 | 🌐 Lua | 📅 2026-08-06 - A Lua implementation of `nvim-hlchunk`, contains more features, such as highlight `{}` chunk, indent line, space blank etc.
* [NMAC427/guess-indent.nvim](https://github.com/NMAC427/guess-indent.nvim) ⭐ 656 | 🐛 18 | 🌐 Lua | 📅 2025-03-25 - Automatic indentation style detection.
* [nvimdev/indentmini.nvim](https://github.com/nvimdev/indentmini.nvim) ⭐ 284 | 🐛 2 | 🌐 Lua | 📅 2026-01-04 - A minimal and blazing fast indentline plugin by using the `nvim_set_decoration_provide` API function.
* [saghen/blink.indent](https://github.com/saghen/blink.indent) ⭐ 232 | 🐛 5 | 🌐 Lua | 📅 2026-06-19 - Performant indent guides with scope on every keystroke.
* [Darazaki/indent-o-matic](https://github.com/Darazaki/indent-o-matic) ⭐ 209 | 🐛 0 | 🌐 Lua | 📅 2026-07-24 - Dumb automatic fast indentation detection written in Lua.
* [VidocqH/auto-indent.nvim](https://github.com/VidocqH/auto-indent.nvim) ⭐ 91 | 🐛 0 | 🌐 Lua | 📅 2023-11-03 - Auto indent cursor when cursor at the first column and press `<TAB>` key like VSCode.
* [gh-liu/fold\_line.nvim](https://github.com/gh-liu/fold_line.nvim) ⭐ 57 | 🐛 0 | 🌐 Lua | 📅 2026-08-06 - Lines for indicating code folding, which could achieve an effect similar to indentline by `:set fdm=indent`.
* [yaocccc/nvim-hlchunk](https://github.com/yaocccc/nvim-hlchunk) ⭐ 54 | 🐛 1 | 🌐 Vim Script | 📅 2025-08-18 - Highlight a `{}` chunk.
* [Mr-LLLLL/cool-chunk.nvim](https://github.com/Mr-LLLLL/cool-chunk.nvim) ⭐ 26 | 🐛 1 | 🌐 Lua | 📅 2025-01-10 - Simpler and faster chunking with animations.
* [LucasTavaresA/simpleIndentGuides.nvim](https://github.com/LucasTavaresA/simpleIndentGuides.nvim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2024-11-24 - Indentation guides using the built-in variables.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Command Line

* [nvim-mini/mini.nvim#mini.cmdline](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-cmdline.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for command line tweaks. Adds autocompletion with customizable delay, autocorrection for words with fixed candidates, and autopeek command range in a floating window.
* [gelguy/wilder.nvim](https://github.com/gelguy/wilder.nvim) ⭐ 1,479 | 🐛 66 | 🌐 Vim script | 📅 2024-07-17 - A plugin for fuzzy command line autocompletion.
* [notomo/cmdbuf.nvim](https://github.com/notomo/cmdbuf.nvim) ⭐ 142 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - Alternative command-line-window plugin.
* [vzze/cmdline.nvim](https://github.com/vzze/cmdline.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2025-04-03 - Helix-like command line with fuzzy autocompletion.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Session

* [nvim-mini/mini.nvim#mini.sessions](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-sessions.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for session management (read, write, delete).
* [rmagatti/auto-session](https://github.com/rmagatti/auto-session) ⭐ 1,854 | 🐛 15 | 🌐 Lua | 📅 2026-08-15 - A small automated session manager.
* [folke/persistence.nvim](https://github.com/folke/persistence.nvim) ⭐ 1,007 | 🐛 9 | 🌐 Lua | 📅 2025-10-28 - Simple automated session management.
* [Shatur/neovim-session-manager](https://github.com/Shatur/neovim-session-manager) ⭐ 617 | 🐛 16 | 🌐 Lua | 📅 2026-01-26 - A simple wrapper around :mksession.
* [olimorris/persisted.nvim](https://github.com/olimorris/persisted.nvim) ⭐ 543 | 🐛 0 | 🌐 Lua | 📅 2026-04-11 - Simple session management with Git branching, autosave/autoload and Telescope support.
* [jedrzejboczar/possession.nvim](https://github.com/jedrzejboczar/possession.nvim) ⭐ 399 | 🐛 13 | 🌐 Lua | 📅 2025-10-21 - Flexible session management with arbitrary persistent data stored as JSON.
* [coffebar/neovim-project](https://github.com/coffebar/neovim-project) ⭐ 301 | 🐛 4 | 🌐 Lua | 📅 2026-05-01 - Declarative project management, automatic saving of sessions, uses Telescope.
* [gennaro-tedesco/nvim-possession](https://github.com/gennaro-tedesco/nvim-possession) ⭐ 289 | 🐛 3 | 🌐 Lua | 📅 2026-03-06 - The no-nonsense session manager.
* [niuiic/multiple-session.nvim](https://github.com/niuiic/multiple-session.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2024-05-25 - Provides multi-session management capabilities.
* [dmshvedchenko/persist.nvim](https://github.com/dmshvedchenko/persist.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-07-27 - Lightweight session persistence with interactive recovery of unnamed scratch buffers.
* [Akmadan23/local-session.nvim](https://github.com/Akmadan23/local-session.nvim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-01-26 - A fast, minimal and implicit current-working-directory-based session manager with easy to configure session files in Lua.
* [njayman/season.nvim](https://github.com/njayman/season.nvim) ⭐ 4 | 🐛 0 | 🌐 Lua | 📅 2025-11-24 - A lightweight plugin to manage session based on current working directory.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Remote Development

* [chipsenkbeil/distant.nvim](https://github.com/chipsenkbeil/distant.nvim) ⭐ 1,369 | 🐛 26 | 🌐 Lua | 📅 2024-10-17 - Edit files, run programs, and work with LSP on a remote machine from the comfort of your local environment.
* [jamestthompson3/nvim-remote-containers](https://github.com/jamestthompson3/nvim-remote-containers) ⭐ 934 | 🐛 11 | 🌐 Lua | 📅 2023-12-22 - Develop inside Docker containers, just like VSCode.
* [esensar/nvim-dev-container](https://github.com/esensar/nvim-dev-container) ⭐ 733 | 🐛 10 | 🌐 Lua | 📅 2026-05-12 - Provide functionality similar to VSCode's [remote container development](https://code.visualstudio.com/docs/remote/containers) plugin, with other functionalities that enable development in Docker containers.
* [nosduco/remote-sshfs.nvim](https://github.com/nosduco/remote-sshfs.nvim) ⭐ 424 | 🐛 21 | 🌐 Lua | 📅 2026-04-05 - Explore, edit, and develop on a remote machine via SSHFS.
* [miversen33/netman.nvim](https://github.com/miversen33/netman.nvim) ⭐ 379 | 🐛 52 | 🌐 Lua | 📅 2025-09-13 - Lua powered Network Resource Manager.
* [azratul/live-share.nvim](https://github.com/azratul/live-share.nvim) ⭐ 275 | 🐛 0 | 🌐 Lua | 📅 2026-07-31 - Provides remote collaboration capabilities from anywhere, making it ideal for pair-programming scenarios.
* [uhs-robert/sshfs.nvim](https://github.com/uhs-robert/sshfs.nvim) ⭐ 162 | 🐛 5 | 🌐 Lua | 📅 2026-05-07 - Mount remote systems via SSHFS with smart picker auto-detect (Telescope/Oil/Snacks/Neo-tree/fzf-lua/Yazi/Ranger etc.).
* [inhesrom/remote-ssh.nvim](https://github.com/inhesrom/remote-ssh.nvim) ⭐ 128 | 🐛 1 | 🌐 Lua | 📅 2026-02-23 - Duplicates the basic ground level functionality of VSCode's Remote-SSH plugin, with a focus on a local editing experience to avoid remote "lag". Browse remote files, edit "remote buffers" with a full local editing experience (LSP, Tree-sitter, Telescope integration, and a file watcher).
* [niuiic/remote.nvim](https://github.com/niuiic/remote.nvim) ⭐ 46 | 🐛 0 | 🌐 Lua | 📅 2024-05-11 - Edit remote files with local configuration.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Live Preview

* [kiyoon/jupynium.nvim](https://github.com/kiyoon/jupynium.nvim) ⭐ 774 | 🐛 12 | 🌐 Python | 📅 2026-04-22 - Selenium-automated Jupyter Notebook with real-time synchronization.
* [gruvw/strudel.nvim](https://github.com/gruvw/strudel.nvim) ⭐ 474 | 🐛 4 | 🌐 JavaScript | 📅 2026-04-10 - Live coding controller for [strudel](https://strudel.cc).
* [brianhuster/live-preview.nvim](https://github.com/brianhuster/live-preview.nvim) ⭐ 418 | 🐛 28 | 🌐 Lua | 📅 2026-08-16 - Live preview HTML, Markdown and Asciidoc in the browser.
* [SUSTech-data/neopyter](https://github.com/SUSTech-data/neopyter) ⭐ 173 | 🐛 3 | 🌐 Lua | 📅 2026-05-20 - Edit and preview/run in Jupyter Lab.
* [hat0uma/prelive.nvim](https://github.com/hat0uma/prelive.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2025-10-05 - A simple luv-based development server with live reloading.
* [ritschalex/jupyter\_ascending.nvim](https://github.com/RitschAlex/jupyter_ascending.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2026-06-27 - A seamless way to work with Jupyter Notebooks using Jupyter Ascending.
* [hat0uma/doxygen-previewer.nvim](https://github.com/hat0uma/doxygen-previewer.nvim) ⭐ 7 | 🐛 1 | 🌐 Lua | 📅 2025-09-17 - Live previewing of Doxygen documentation.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Split and Window

* [nvim-mini/mini.nvim#mini.bufremove](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-bufremove.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for buffer removing (unshow, delete, wipeout) while saving window layout.
* [mrjones2014/smart-splits.nvim](https://github.com/mrjones2014/smart-splits.nvim) ⭐ 1,711 | 🐛 20 | 🌐 Lua | 📅 2026-08-14 - Smart, seamless, directional navigation and resizing of splits.
* [nvim-focus/focus.nvim](https://github.com/nvim-focus/focus.nvim) ⭐ 812 | 🐛 24 | 🌐 Lua | 📅 2026-02-08 - Auto-Focusing and Auto-Resizing Splits/Windows written in Lua! Vim splits on steroids.
* [nvim-zh/colorful-winsep.nvim](https://github.com/nvim-zh/colorful-winsep.nvim) ⭐ 706 | 🐛 0 | 🌐 Lua | 📅 2026-04-26 - A configurable color split line.
* [anuvyklack/windows.nvim](https://github.com/anuvyklack/windows.nvim) ⭐ 640 | 🐛 22 | 🌐 Lua | 📅 2023-07-08 - Automatically expand width of the current window. Maximizes and restore it. And all this with nice animations.
* [sindrets/winshift.nvim](https://github.com/sindrets/winshift.nvim) ⭐ 528 | 🐛 9 | 🌐 Lua | 📅 2024-05-20 - Rearrange your windows with ease.
* [altermo/nwm](https://github.com/altermo/nwm) ⭐ 349 | 🐛 1 | 🌐 Lua | 📅 2026-05-20 - X11 window manager.
* [yorickpeterse/nvim-window](https://github.com/yorickpeterse/nvim-window) ⭐ 186 | 🐛 0 | 🌐 Lua | 📅 2026-01-20 - Easily jump between windows.
* [nyngwang/NeoNoName.lua](https://github.com/nyngwang/NeoNoName.lua) ⭐ 29 | 🐛 2 | 🌐 Lua | 📅 2023-06-01 - Layout preserving buffer deletion.
* [jyscao/ventana.nvim](https://github.com/jyscao/ventana.nvim) ⭐ 24 | 🐛 0 | 🌐 Lua | 📅 2025-11-23 - Convenient flips and shifts for your windows layout.
* [wsdjeg/tabman.nvim](https://github.com/wsdjeg/tabman.nvim) ⭐ 18 | 🐛 1 | 🌐 Lua | 📅 2026-07-21 - Navigate between tabs and the windows they contain.
* [MisanthropicBit/winmove.nvim](https://github.com/MisanthropicBit/winmove.nvim) ⭐ 16 | 🐛 2 | 🌐 Lua | 📅 2026-04-02 - Easily move, swap, and resize windows.
* [aronjohanns/smooth-resize.nvim](https://github.com/aronjohanns/smooth-resize.nvim) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2026-01-23 - Smooth, continuous window resizing with the default window resizing mappings.
* [ycdzj/win-mover.nvim](https://github.com/ycdzj/win-mover.nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-04-14 - Window mover that avoids moving side windows.
* [mkajsjo/windowcolumns.nvim](https://github.com/mkajsjo/windowcolumns.nvim) ⭐ 8 | 🐛 0 | 🌐 Lua | 📅 2025-06-07 - Column-first window management.
* [\~henriquehbr/ataraxis.lua](https://sr.ht/~henriquehbr/ataraxis.lua) - A zen mode for improving code readability.

### Tmux

* [aserowy/tmux.nvim](https://github.com/aserowy/tmux.nvim) ⭐ 809 | 🐛 16 | 🌐 Lua | 📅 2026-04-13 - Tmux integration features pane movement and resizing.
* [hkupty/nvimux](https://github.com/hkupty/nvimux) ⭐ 450 | 🐛 4 | 🌐 Lua | 📅 2022-05-19 - Use your editor as a tmux replacement.
* [numToStr/Navigator.nvim](https://github.com/numToStr/Navigator.nvim) ⭐ 434 | 🐛 14 | 🌐 Lua | 📅 2024-07-07 - Smoothly navigate between editor splits and tmux panes.
* [declancm/windex.nvim](https://github.com/declancm/windex.nvim) ⭐ 62 | 🐛 1 | 🌐 Lua | 📅 2022-07-12 - Collection of window functions which includes moving between, closing and maximizing editor splits and tmux panes.
* [EvWilson/slimux.nvim](https://github.com/EvWilson/slimux.nvim) ⭐ 34 | 🐛 0 | 🌐 Lua | 📅 2025-11-13 - Send content from the current buffer to a configurable tmux pane.
* [danielpieper/telescope-tmuxinator.nvim](https://github.com/danielpieper/telescope-tmuxinator.nvim) ⭐ 26 | 🐛 0 | 🌐 Lua | 📅 2023-12-17 - Integration for tmuxinator with telescope.nvim.
* [kiyoon/tmux-send.nvim](https://github.com/kiyoon/tmux-send.nvim) ⭐ 23 | 🐛 0 | 🌐 Lua | 📅 2026-01-24 - Copy and paste buffer content or file path in either `nvim-tree`, `neo-tree` or `oil.nvim` to another tmux pane.
* [juselara1/tmutils.nvim](https://github.com/juselara1/tmutils.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2024-12-21 - Tmux utilities that enable sending lines, capturing content, creating terminals, and managing REPLs.
* [karnull/only-tmux.nvim](https://github.com/karnull/only-tmux.nvim) ⭐ 17 | 🐛 0 | 🌐 Lua | 📅 2026-06-13 - Expand the functionality of `:only` with tmux panes in the same window, with either moving them to a new window or closing them.
* [salorak/libtmux.nvim](https://github.com/salorak/libtmux.nvim) ⭐ 9 | 🐛 0 | 🌐 Lua | 📅 2026-02-15 - Thin wrapper for using the `tmux` API.
* [jkeresman01/tmux-switch.nvim](https://github.com/jkeresman01/tmux-switch.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-10-09 - Provides fuzzy session switching for Tmux.
* [karshPrime/tmux-compile.nvim](https://github.com/karshPrime/tmux-compile.nvim) ⭐ 1 | 🐛 0 | 🌐 Lua | 📅 2026-06-13 - Set up same key, like F5, to run any compile/run command per language, like `make` for C and `cargo build` for Rust, and have the project run or compile in a new tmux pane or window.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Game

* [Eandrju/cellular-automaton.nvim](https://github.com/Eandrju/cellular-automaton.nvim) ⭐ 2,096 | 🐛 13 | 🌐 Lua | 📅 2025-01-31 - It lets you execute aesthetically pleasing, cellular automaton animations based on the content of the current buffer.
* [alec-gibson/nvim-tetris](https://github.com/alec-gibson/nvim-tetris) ⭐ 216 | 🐛 7 | 🌐 Lua | 📅 2024-01-17 - Bringing Emacs' greatest feature - Tetris.
* [seandewar/actually-doom.nvim](https://github.com/seandewar/actually-doom.nvim) ⭐ 140 | 🐛 3 | 🌐 C | 📅 2026-04-15 - Editing text is boring; play DOOM instead!.
* [seandewar/nvimesweeper](https://github.com/seandewar/nvimesweeper) ⭐ 112 | 🐛 1 | 🌐 Lua | 📅 2024-06-29 - Play Minesweeper in your favourite text editor.
* [rktjmp/playtime.nvim](https://github.com/rktjmp/playtime.nvim) ⭐ 93 | 🐛 1 | 🌐 Fennel | 📅 2026-07-16 - A collection of games such as Freecell, Shenzhen Solitaire and The Emissary.
* [jim-fx/sudoku.nvim](https://github.com/jim-fx/sudoku.nvim) ⭐ 79 | 🐛 1 | 🌐 Lua | 📅 2023-12-11 - Classic sudoku puzzle.
* [seandewar/killersheep.nvim](https://github.com/seandewar/killersheep.nvim) ⭐ 75 | 🐛 1 | 🌐 Lua | 📅 2025-03-20 - A port of killersheep.
* [alanfortlink/blackjack.nvim](https://github.com/alanfortlink/blackjack.nvim) ⭐ 73 | 🐛 0 | 🌐 Lua | 📅 2026-05-21 - Classic Black Jack game.
* [piersolenski/skifree.nvim](https://github.com/piersolenski/skifree.nvim) ⭐ 18 | 🐛 0 | 🌐 Lua | 📅 2025-11-24 - Play the Windows 3.1 SkiFree game.
* [xiangnongWu2233/rubiks-cube.nvim](https://github.com/xiangnongWu2233/rubiks-cube.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2026-06-11 - A playable Rubik's cube with auto-solver.
* [csessh/aoc.vim](https://github.com/csessh/aoc.nvim) ⭐ 9 | 🐛 1 | 🌐 Lua | 📅 2025-12-01 - Simple little elf who fetches Advent of Code puzzle input for you.

### Competitive Programming

* [kawre/leetcode.nvim](https://github.com/kawre/leetcode.nvim) ⭐ 2,145 | 🐛 64 | 🌐 Lua | 📅 2026-04-28 - Solve Leetcode problems.
* [xeluxee/competitest.nvim](https://github.com/xeluxee/competitest.nvim) ⭐ 596 | 🐛 21 | 🌐 Lua | 📅 2025-05-13 - A plugin to automate testcases management and checking for Competitive Programming contests.
* [2KAbhishek/exercism.nvim](https://github.com/2KAbhishek/exercism.nvim) ⭐ 48 | 🐛 0 | 🌐 Lua | 📅 2026-03-12 - Browse and solve Exercism problems.
* [\~chinmay/cphelper.nvim](https://git.sr.ht/~chinmay/cphelper.nvim) - Helper for competitive programming written in Lua.
* [barrettruth/cp.nvim](https://github.com/barrettruth/cp.nvim) - Competitive programming workflow for popular contest platforms (CodeForces, CSES, etc.) Includes automatic test scraping, I/O view, and diff panel.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Toys

* [folke/drop.nvim](https://github.com/folke/drop.nvim) ⭐ 350 | 🐛 2 | 🌐 Lua | 📅 2025-10-28 - Screensavers with support for dashboards.
* [axsaucedo/neovim-power-mode](https://github.com/axsaucedo/neovim-power-mode) ⭐ 99 | 🐛 2 | 🌐 Lua | 📅 2026-08-08 - Combo counter, particle effects and explosions for your editor.
* [jerrywang1981/keystroke.nvim](https://github.com/jerrywang1981/keystroke.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2025-04-01 - Play sounds and do other things as you type.
* [cxwx/keywound.nvim](https://github.com/cxwx/keysound.nvim) ⭐ 2 | 🐛 0 | 🌐 Lua | 📅 2026-04-30 - Play a sound on each keystroke, supports customizable sounds.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Workflow

* [m4xshen/hardtime.nvim](https://github.com/m4xshen/hardtime.nvim) ⭐ 3,838 | 🐛 15 | 🌐 Lua | 📅 2026-07-20 - Helping you establish good command workflow and habit.
* [saxon1964/neovim-tips](https://github.com/saxon1964/neovim-tips) ⭐ 469 | 🐛 2 | 🌐 Lua | 📅 2026-04-19 - Provides hundreds of built-in tips, tricks and shortcuts, with a custom picker interface and the ability to add your own tips.
* [ecthelionvi/NeoComposer.nvim](https://github.com/ecthelionvi/NeoComposer.nvim) ⚠️ Archived - Simplify macro management, enhance productivity, and create harmonious workflows.
* [letieu/jira.nvim](https://github.com/letieu/jira.nvim) ⭐ 266 | 🐛 7 | 🌐 Lua | 📅 2026-07-21 - Manage Jira tasks with a beautiful UI.
* [jghauser/mkdir.nvim](https://github.com/jghauser/mkdir.nvim) ⭐ 230 | 🐛 1 | 🌐 Lua | 📅 2022-07-23 - Automatically create missing directories when saving files.
* [emrearmagan/atlas.nvim](https://github.com/emrearmagan/atlas.nvim) ⭐ 209 | 🐛 11 | 🌐 Lua | 📅 2026-08-16 - A single workflow for GitHub, GitLab, Bitbucket, and Jira.
* [mateuszwieloch/automkdir.nvim](https://github.com/mateuszwieloch/automkdir.nvim) ⭐ 32 | 🐛 0 | 🌐 Lua | 📅 2025-03-31 - Automatically create non-existent parent directories when writing a file.
* [yagiziskirik/AirSupport.nvim](https://github.com/yagiziskirik/AirSupport.nvim) ⭐ 11 | 🐛 0 | 🌐 Lua | 📅 2023-05-25 - Searchable reminder window for your custom shortcuts and commands.

### Stats Tracking

* [gisketch/triforce.nvim](https://github.com/gisketch/triforce.nvim) ⭐ 305 | 🐛 0 | 🌐 Lua | 📅 2026-08-11 - Gamified stat tracker with XP, levels, achievements, and activity heatmaps for your coding sessions with lualine integration.
* [aikhe/wrapped.nvim](https://github.com/aikhe/wrapped.nvim) ⭐ 185 | 🐛 0 | 🌐 Lua | 📅 2026-06-28 - Visualize and review your configuration activity with stats, insights, history, heatmaps and more.
* [gaborvecsei/usage-tracker.nvim](https://github.com/gaborvecsei/usage-tracker.nvim) ⭐ 144 | 🐛 3 | 🌐 Lua | 📅 2024-03-10 - Track your usage and visualize statistics easily.
* [ptdewey/pendulum-nvim](https://github.com/ptdewey/pendulum-nvim) ⭐ 113 | 🐛 1 | 🌐 Go | 📅 2026-07-10 - Track time spent coding and glean insights through on-demand time reports.
* [Rtarun3606k/takatime](https://github.com/Rtarun3606k/takatime) ⭐ 102 | 🐛 50 | 🌐 Go | 📅 2026-08-16 - Privacy-first WakaTime alternative using Go and MongoDB.
* [QuentinGruber/pomodoro.nvim](https://github.com/QuentinGruber/pomodoro.nvim) ⭐ 49 | 🐛 1 | 🌐 Lua | 📅 2025-11-24 - Use the Pomodoro Technique with built-in session tracking and break reminders.
* [ravsii/timers.nvim](https://github.com/ravsii/timers.nvim) ⭐ 18 | 🐛 1 | 🌐 Lua | 📅 2025-10-13 - Timer manager, a clean Lua API, supporting multiple timers, persistence, UI, and plugin integrations.
* [SunnyTamang/pendulum.nvim](https://github.com/SunnyTamang/pendulum.nvim) ⭐ 14 | 🐛 1 | 🌐 Lua | 📅 2024-08-22 - Simple timer for creating time based productive sessions for coders, competitive programmers, developers etc.
* [yal212/pomodoro.nvim](https://github.com/yal212/pomodoro.nvim) ⭐ 5 | 🐛 0 | 🌐 Lua | 📅 2026-07-11 - Focus-first Pomodoro timer with automatic work, break cycles, session statistics, and a distraction-free focus mode.
* [raymondware/focusmode.nvim](https://github.com/raymondware/focusmode.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-07-30 - Pomodoro and deep-work timer with configurable intervals, distraction blocking, session statistics, and a dashboard.
* [taigrr/blast.nvim](https://github.com/taigrr/blast.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-08-08 - Activity tracking client for NvimBlast with per-project configuration, monorepo support, and privacy controls.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Database

* [kndndrj/nvim-dbee](https://github.com/kndndrj/nvim-dbee) ⭐ 1,291 | 🐛 77 | 🌐 Go | 📅 2025-07-25 - Interactive database client.
* [joryeugene/dadbod-grip.nvim](https://github.com/joryeugene/dadbod-grip.nvim) ⭐ 164 | 🐛 3 | 🌐 Lua | 📅 2026-07-31 - Database editor with inline cell editing, staged mutations with live SQL preview, schema browser, DDL, AI SQL generation, FK navigation, and DuckDB/Parquet support.
* [zongben/dbout.nvim](https://github.com/zongben/dbout.nvim) ⭐ 42 | 🐛 0 | 🌐 Lua | 📅 2026-07-08 - Manage database connections and run SQL queries directly with JSON results.
* [tashikomaaa/neomongo.nvim](https://github.com/tashikomaaa/neomongo.nvim) ⭐ 8 | 🐛 1 | 🌐 Lua | 📅 2025-11-03 - Explore, query, and edit MongoDB collections directly through a Telescope-powered dashboard.
* [clang-engineer/dadbod-vertica.nvim](https://github.com/clang-engineer/dadbod-vertica.nvim) ⭐ 2 | 🐛 0 | 🌐 Vim Script | 📅 2026-07-06 - Vertica adapter for [vim-dadbod](https://github.com/tpope/vim-dadbod) ⭐ 4,429 | 🐛 58 | 🌐 Vim Script | 📅 2026-01-07 via the official `vsql` client, with schema-tree integration for `vim-dadbod-ui`.
* [zerochae/dbab.nvim](https://github.com/zerochae/dbab.nvim) - Lightweight database client with a modern UI and async execution.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Pre-made Configuration

* [pgosar/CyberNvim](https://github.com/pgosar/CyberNvim) ⭐ 380 | 🐛 2 | 🌐 Lua | 📅 2025-02-20 - The world's simplest and most extensible Neovim distribution.
* [Abstract-IDE/Abstract](https://github.com/Abstract-IDE/Abstract) ⭐ 212 | 🐛 2 | 🌐 Lua | 📅 2026-07-18 - Configuration to achieve the power of Modern IDE.
* [tokiory/neovim-boilerplate](https://github.com/tokiory/neovim-boilerplate) ⭐ 133 | 🐛 0 | 🌐 Lua | 📅 2025-06-23 - Starter boilerplate for making new configurations.
* [frans-johansson/lazy-nvim-starter](https://github.com/frans-johansson/lazy-nvim-starter) ⭐ 100 | 🐛 1 | 🌐 Lua | 📅 2023-10-26 - Starter boilerplate with lazy plugin manager.
* [sontungexpt/stinvim](https://github.com/sontungexpt/stinvim) ⭐ 53 | 🐛 1 | 🌐 Lua | 📅 2026-02-22 - Configuration for Full-Stack developers.
* [abdellatif-temsamani/adev.nvim](https://github.com/abdellatif-temsamani/adev.nvim) ⭐ 10 | 🐛 3 | 🌐 Lua | 📅 2026-08-06 - The over-engineered Neovim distribution for developers who want everything.

<!--lint disable double-link -->

* [SpaceVim/SpaceVim](https://spacevim.org) - A community-driven modular distribution, inspired by [spacemacs](https://github.com/syl20bnr/spacemacs) ⭐ 24,575 | 🐛 64 | 🌐 Emacs Lisp | 📅 2026-08-11.

<!--lint enable double-link -->

* [nvim-lua/kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim) ⭐ 31,277 | 🐛 22 | 🌐 Lua | 📅 2026-08-07 - A launch point for your personal configuration.
* [siduck76/NvChad](https://github.com/siduck76/NvChad) ⭐ 28,436 | 🐛 3 | 🌐 Lua | 📅 2026-07-03 - An attempt to make the built-in CLI as functional as an IDE while retaining beauty with less bloat.
* [LazyVim/LazyVim](https://github.com/LazyVim/LazyVim) ⭐ 27,171 | 🐛 77 | 🌐 Lua | 📅 2026-06-02 - Full-fledged IDE powered by **lazy.nvim** to make it easy to customize and extend your config.
* [LunarVim/LunarVim](https://github.com/LunarVim/LunarVim) ⭐ 19,275 | 🐛 33 | 🌐 Lua | 📅 2025-06-05 - This project aims to help one transition away from VSCode, and into a superior text editing experience.
* [AstroNvim/AstroNvim](https://github.com/AstroNvim/AstroNvim) ⭐ 14,414 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - An aesthetic and feature-rich config that is extensible and easy to use with a great set of plugins.
* [ayamir/nvimdots](https://github.com/ayamir/nvimdots) ⭐ 3,419 | 🐛 3 | 🌐 Lua | 📅 2026-08-15 - A well-configured and structured configuration with NixOS support.
* [shaunsingh/nyoom.nvim](https://github.com/shaunsingh/nyoom.nvim) ⭐ 1,625 | 🐛 30 | 🌐 Fennel | 📅 2023-11-05 - Blazing fast, configurable, minimal and "lispy" config written in Fennel.
* [CosmicNvim/CosmicNvim](https://github.com/CosmicNvim/CosmicNvim) ⭐ 1,161 | 🐛 0 | 🌐 Lua | 📅 2026-08-10 - CosmicNvim is a lightweight and opinionated config for web development, specifically designed to provide a COSMIC programming experience.
* [dam9000/kickstart-modular.nvim](https://github.com/dam9000/kickstart-modular.nvim) ⭐ 1,012 | 🐛 3 | 🌐 Lua | 📅 2026-07-25 - This is a fork of nvim-lua/kickstart.nvim that moves from a single file to a multi file configuration.
* [artart222/CodeArt](https://github.com/artart222/CodeArt) ⭐ 904 | 🐛 0 | 🌐 Lua | 📅 2026-08-07 - A fast general-purpose IDE written entirely in Lua with an installer for Linux/Windows/macOS and built-in `:CodeArtUpdate` command for updating it.
* [ldelossa/nvim-ide](https://github.com/ldelossa/nvim-ide) ⭐ 880 | 🐛 14 | 🌐 Lua | 📅 2025-07-27 - A full featured IDE layer heavily inspired by VSCode.
* [NormalNvim/NormalNvim](https://github.com/NormalNvim/NormalNvim) ⭐ 724 | 🐛 4 | 🌐 Lua | 📅 2026-04-01 - Configuration focused on stability for your daily work.
* [crivotz/nv-ide](https://github.com/crivotz/nv-ide) ⭐ 649 | 🐛 1 | 🌐 Lua | 📅 2026-07-15 - Custom configuration oriented for Full-Stack developers (Rails, Ruby, PHP, HTML, CSS, SCSS, JavaScript).
* [hackorum/VapourNvim](https://github.com/hackorum/VapourNvim) ⭐ 561 | 🐛 17 | 🌐 Lua | 📅 2023-03-31 - Configuration for the ultimate Vim IDE-like experience.
* [nvim-mini/MiniMax](https://github.com/nvim-mini/MiniMax) ⭐ 460 | 🐛 2 | 🌐 Lua | 📅 2026-08-15 - A collection of self-contained and extensively commented configurations which mostly use MINI tools.
* [doctorfree/nvim-lazyman](https://github.com/doctorfree/nvim-lazyman) ⭐ 438 | 🐛 9 | 🌐 HTML | 📅 2025-11-21 - Configuration manager and a modular configuration on its own. Supports over 40 preconfigured configurations.
* [mrcjkb/kickstart-nix.nvim](https://github.com/mrcjkb/kickstart-nix.nvim) ⭐ 405 | 🐛 3 | 🌐 Lua | 📅 2026-04-01 - Template repo for Neovim derivations, with the goal of simplifying the migration from existing configurations.
* [Shaobin-Jiang/IceNvim](https://github.com/Shaobin-Jiang/IceNvim) ⭐ 330 | 🐛 3 | 🌐 Lua | 📅 2026-08-05 - A beautiful, powerful and customizable config that is blazingly fast.
* [shaeinst/roshnivim](https://github.com/shaeinst/roshnivim) ⭐ 212 | 🐛 2 | 🌐 Lua | 📅 2026-07-18 - A predefined config to save you thousands of hours to setup your editor as an IDE.
* [adoyle-h/one.nvim](https://github.com/adoyle-h/one.nvim) ⭐ 187 | 🐛 0 | 🌐 Lua | 📅 2026-04-24 - All-in-one config framework in Lua.
* [chrisgrieser/nvim-kickstart-python](https://github.com/chrisgrieser/nvim-kickstart-python) ⚠️ Archived - A launch point for your configuration (for Python).
* [cstsunfu/.sea.nvim](https://github.com/cstsunfu/.sea.nvim) ⭐ 148 | 🐛 0 | 🌐 Lua | 📅 2026-07-10 - A modular configuration with a beautiful UI and some useful features such as a pomodoro clock and window numbers.
* [linrongbin16/lin.nvim](https://github.com/linrongbin16/lin.nvim) ⭐ 93 | 🐛 0 | 🌐 Lua | 📅 2026-08-13 - A highly configured Neovim distribution integrated with tons of utilities for development, inspired by `spf13-vim`.
* [crispybaccoon/chaivim](https://github.com/crispybaccoon/chaivim) ⚠️ Archived - Easily configurable distro with solid defaults and a cozy editor experience.
* [imbacraft/dusk.nvim](https://github.com/imbacraft/dusk.nvim) ⭐ 54 | 🐛 0 | 🌐 Lua | 📅 2024-06-02 - A lightweight, aesthetically minimal config, written in Lua, able to provide for web and Java development.
* [drybalka/clean.nvim](https://github.com/drybalka/clean.nvim) ⭐ 41 | 🐛 0 | 🌐 Lua | 📅 2024-01-29 - Cleaning up the default key mappings and plugins and leaving only the bare essentials to build upon.
* [legobeat/l7-devenv](https://github.com/legobeat/l7-devenv) ⭐ 27 | 🐛 34 | 🌐 JavaScript | 📅 2025-12-01 - Security-focused IDE with a hackable (in the right way) framework based on Neovim and shell.
* [StratOS-Linux/StratVIM](https://github.com/StratOS-Linux/StratVIM) ⭐ 16 | 🐛 1 | 🌐 Lua | 📅 2026-07-29 - A full-fledged Neovim distribution included by default in [StratOS-Linux](https://github.com/StratOS-Linux).
* [cunderw/nvim](https://github.com/cunderw/nvim) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2024-04-02 - A custom, IDE-like configuration for JS/TS, Go, and Java development.
* [plutowang/nvim.pack](https://github.com/plutowang/nvim.pack) ⭐ 12 | 🐛 0 | 🌐 Lua | 📅 2026-08-06 - Declarative, event-driven lazy-loading configuration built purely on native Vim.pack for extreme startup performance.
* [jrychn/moduleVim](https://github.com/jrychn/ModuleVim) ⭐ 10 | 🐛 0 | 🌐 Lua | 📅 2025-10-31 - A very easy to use for backend and frontend, install LSP automatically.
* [TheItcor/MoaiVim](https://github.com/TheItcor/MoaiVim) ⭐ 7 | 🐛 0 | 🌐 Lua | 📅 2026-03-09 - A minimalist config that emulates a lightweight IDE.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## External

These tools are used externally to Neovim to enhance the experience.

### Version Manager

* [MordechaiHadad/bob](https://github.com/MordechaiHadad/bob) ⭐ 2,136 | 🐛 20 | 🌐 Rust | 📅 2026-08-16 - A cross-platform, easy to use version manager.
* [NTBBloodbath/nvenv](https://github.com/NTBBloodbath/nvenv) ⭐ 61 | 🐛 2 | 🌐 V | 📅 2025-05-14 - A lightweight and blazingly fast version manager.
* [y3owk1n/nvs](https://github.com/y3owk1n/nvs) ⭐ 38 | 🐛 0 | 🌐 Go | 📅 2026-08-16 - Another version manager with config switcher.

### Plugin Template

* [ellisonleao/nvim-plugin-template](https://github.com/ellisonleao/nvim-plugin-template) ⭐ 473 | 🐛 2 | 🌐 Lua | 📅 2025-10-08 - Another plugin template, using GitHub's template feature.
* [m00qek/plugin-template.nvim](https://github.com/m00qek/plugin-template.nvim) ⭐ 135 | 🐛 2 | 🌐 Lua | 📅 2023-12-17 - A plugin template that setups test infrastructure and GitHub Actions.
* [gennaro-tedesco/boilit](https://github.com/gennaro-tedesco/boilit) ⭐ 86 | 🐛 0 | 🌐 Go | 📅 2022-11-22 - Create boilerplate structure plugins.
* [chrisgrieser/nvim-pseudometa-plugin-template](https://github.com/chrisgrieser/nvim-pseudometa-plugin-template) ⭐ 41 | 🐛 2 | 🌐 Shell | 📅 2026-06-22 - Template for new plugins.
* [jkeresman01/spring-initializr.nvim](https://github.com/jkeresman01/spring-initializr.nvim) ⭐ 21 | 🐛 60 | 🌐 Lua | 📅 2026-07-12 - Scaffold Spring Boot projects with a Telescope-powered UI.
* [2KAbhishek/template.nvim](https://github.com/2KAbhishek/template.nvim) ⭐ 19 | 🐛 0 | 🌐 Lua | 📅 2025-08-05 - Opinionated template for starting plugin dev quickly.
* [DrKJeff16/nvim-plugin-boilerplate](https://github.com/DrKJeff16/nvim-plugin-boilerplate) ⭐ 15 | 🐛 0 | 🌐 Shell | 📅 2026-08-12 - A documented template for new plugins generated by a script. Includes tests, CI utilities, etc.

### OS-specific

* [iamironz/android-nvim-plugin](https://github.com/iamironz/android-nvim-plugin) ⭐ 81 | 🐛 6 | 🌐 Lua | 📅 2026-03-25 - Android build, deploy, and logcat commands with Gradle integration.
* [m15a/flake-awesome-neovim-plugins](https://github.com/m15a/flake-awesome-neovim-plugins) ⭐ 62 | 🐛 0 | 🌐 Nix | 📅 2026-08-15 - Nix flake that provides a collection of `awesome-neovim` plugins as Nix packages.
* [chrisgrieser/alfred-neovim-utilities](https://github.com/chrisgrieser/alfred-neovim-utilities) ⭐ 45 | 🐛 0 | 🌐 JavaScript | 📅 2026-08-15 - Search plugins and online `:help` via Alfred (macOS).
* [massix/termux.nvim](https://github.com/massix/termux.nvim) ⭐ 28 | 🐛 1 | 🌐 Lua | 📅 2024-02-22 - Interact with Termux APIs, useful to gather various information about your Android phone to display in the statusline (e.g. battery level).

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## Wishlist

Have a problem a plugin can solve? Add it to the [nvim-lua wishlist](https://github.com/nvim-lua/wishlist) ⭐ 251 | 🐛 39 | 📅 2020-09-29.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## UI

* [nvim-mini/mini.nvim#mini.notify](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-notify.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` to show one or more highlighted notifications in a single window. Provides maker of `vim.notify()` implementation and sets up automated LSP progress updates.
* [nvim-mini/mini.nvim#mini.input](https://github.com/nvim-mini/mini.nvim/blob/main/readmes/mini-input.md) ⭐ 9,448 | 🐛 34 | 🌐 Lua | 📅 2026-08-15 - Module of `mini.nvim` for getting user input with fully customizable key and view handling. Can show as floating window, statusline/tabline/winbar, virtual line/text. Provides `vim.ui.input()` implementation.
* [folke/noice.nvim](https://github.com/folke/noice.nvim) ⭐ 5,803 | 🐛 33 | 🌐 Lua | 📅 2025-11-03 - Highly experimental plugin that completely replaces the UI for messages, cmdline and the popupmenu.
* [rcarriga/nvim-notify](https://github.com/rcarriga/nvim-notify) ⭐ 3,568 | 🐛 80 | 🌐 Lua | 📅 2025-09-06 - A fancy, configurable, notification manager.
* [mcauley-penney/visual-whitespace.nvim](https://github.com/mcauley-penney/visual-whitespace.nvim) ⭐ 477 | 🐛 0 | 🌐 Lua | 📅 2026-06-05 - See whitespace characters in Visual selections, like VSCode.
* [ghillb/cybu.nvim](https://github.com/ghillb/cybu.nvim) ⭐ 327 | 🐛 0 | 🌐 Lua | 📅 2026-05-03 - Displays a notification window with context when cycling buffers.
* [LukasPietzschmann/telescope-tabs](https://github.com/LukasPietzschmann/telescope-tabs) ⚠️ Archived - Quickly navigate between tabs using telescope.
* [matbme/JABS.nvim](https://github.com/matbme/JABS.nvim) ⭐ 283 | 🐛 12 | 🌐 Lua | 📅 2023-05-28 - Pretty and minimal buffer switcher window.
* [toppair/reach.nvim](https://github.com/toppair/reach.nvim) ⭐ 243 | 🐛 5 | 🌐 Lua | 📅 2022-11-21 - Buffer, mark, tabpage switcher.
* [sitiom/nvim-numbertoggle](https://github.com/sitiom/nvim-numbertoggle) ⭐ 229 | 🐛 4 | 🌐 Lua | 📅 2026-06-19 - Automatically toggle between relative and absolute line numbers.
* [CosmicNvim/cosmic-ui](https://github.com/CosmicNvim/cosmic-ui) ⭐ 170 | 🐛 0 | 🌐 Lua | 📅 2026-08-11 - Cosmic-UI is a simple wrapper around specific Vim functionality.
* [OXY2DEV/ui.nvim](https://github.com/OXY2DEV/ui.nvim) ⭐ 158 | 🐛 3 | 🌐 Lua | 📅 2026-02-14 - A blueprint/template/guide for customizing the UI.
* [jrop/tuis.nvim](https://github.com/jrop/tuis.nvim) ⭐ 148 | 🐛 0 | 🌐 Lua | 📅 2026-01-15 - A collection of interactive TUIs which provides rich, interactive UIs to various CLIs.
* [xieyonn/spinner.nvim](https://github.com/xieyonn/spinner.nvim) ⭐ 99 | 🐛 2 | 🌐 Lua | 📅 2026-03-16 - Extensible spinner framework for animated spinners in statusline, tabline, winbar, buffer, cmdline, or next to the cursor.
* [ariel-frischer/bmessages.nvim](https://github.com/ariel-frischer/bmessages.nvim) ⭐ 60 | 🐛 3 | 🌐 Lua | 📅 2025-01-10 - Replace the default `:messages` window with a configurable, auto-updating buffer.
* [wsdjeg/calendar.nvim](https://github.com/wsdjeg/calendar.nvim) ⭐ 52 | 🐛 1 | 🌐 Lua | 📅 2026-07-16 - A simple floating calendar with extensions support.
* [nkakouros-original/numbers.nvim](https://github.com/nkakouros-original/numbers.nvim) ⭐ 41 | 🐛 0 | 🌐 Lua | 📅 2026-04-26 - Toggle relativenumber whenever it makes sense.
* [cpea2506/relative-toggle.nvim](https://github.com/cpea2506/relative-toggle.nvim) ⭐ 37 | 🐛 0 | 🌐 Lua | 📅 2025-07-13 - Toggles smoothly between number and relative numbers, supporting various number combinations, highly customizable.
* [markgandolfo/lightswitch.nvim](https://github.com/markgandolfo/lightswitch.nvim) ⭐ 20 | 🐛 2 | 🌐 Lua | 📅 2025-06-29 - Toggle various options using the `nui.nvim` library.
* [quickui.nvim](https://github.com/mjmjm0101/quickui.nvim) ⭐ 14 | 🐛 0 | 🌐 Lua | 📅 2026-04-26 - Structured, keyboard-driven menus and context menus with nested navigation.
* [ln.nvim](https://github.com/markosnarinian/ln.nvim) ⭐ 3 | 🐛 0 | 🌐 Lua | 📅 2026-06-25 - Relative numbers on the active window, absolute everywhere else.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

## External Resource

* [akrawchyk/awesome-vim#tools](https://github.com/akrawchyk/awesome-vim#tools) ⭐ 2,124 | 🐛 11 | 📅 2025-06-06 - A short list of Vim plugins and helpful guides.
* [Weyaaron/nvim-training](https://github.com/Weyaaron/nvim-training) ⭐ 126 | 🐛 4 | 🌐 Lua | 📅 2026-01-18 - A beginner-friendly tool for training your 'muscle memory' using small, repeatable tasks.
* [ChuYanLon/chad46](https://github.com/ChuYanLon/chad46) ⭐ 8 | 🐛 0 | 🌐 Vim Script | 📅 2026-08-08 - 94 themes with 44 highlight integrations, daily synced from NvChad/base46.
* [Vimawesome](https://vimawesome.com/) - Showcases various plugins for Vim and has a [Neovim tag](https://vimawesome.com/?q=tag:neovim) for other Neovim-related plugins.
* [Neovimcraft](https://neovimcraft.com) - A site dedicated to searching specific plugins and guides for building plugins in Lua.
* [Dotfyle](https://dotfyle.com) - A site for sharing and discovering configurations and plugins.
* [NeoLand](https://neoland.dev) - A beautifully crafted website for Neovim resources.
* [Nvim.app](https://nvim.app) - A modern search interface for plugins with fuzzy search, filtering, and self-service updates for plugin authors.
* [Neovim Cheatsheet](https://neovimcheatsheet.com) - Searchable, interactive cheatsheet with per-keypress search, remappable keybindings, and JSON import/export.

<!--lint disable double-link -->

[**⬆ back to top**](#contents)

<!--lint enable double-link -->

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-16._
