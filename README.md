# Ruby Tools

This plugin naively adds the missing client extensions needed to fully support
codelens in the ruby-lsp. If you are seeing this sort or error:
`Language server`ruby_lsp`does not support command`rubyLsp.openFile`. This command may require a client extension`
this plugin fixes it by implementing missing handlers for:

- `rubyLsp.openFile`
- `rubyLsp.runTest`
- `rubyLsp.debugTest`

You don't need to do anything else to enable opening files, this lets you
navigate around to views and routes in rails quickly using codelenses.

For running tests you'll need to have configured neotest as it's used to run
them.

With lazy, you can install the plugin with one line:

```
{ "Seich/ruby-tools", opts = {}, dependencies = { "nvim-neotest/neotest" } },
```

This is basically built for my own config so there are no options to change. If
you need anything else out of this plugin feel free to open a pr or copy and
paste it and customize it to be your own.

https://github.com/user-attachments/assets/855055a9-a7f5-4756-9e2c-67e5a6cd3251
