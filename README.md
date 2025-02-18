# asdf GitHub Action

GitHub Action that installs and configures [asdf](https://asdf-vm.com/) version >= 0.16.  Cache is used when possible to speed up the install.

Only the asdf binary is installed. You will need to install any needed asdf plugins and then run `asdf install` to actually install all your runtimes defined in your `.tool-versions` file.

This action supports Linux (AMD) and macOS (ARM) runners.

## Example usage

```yaml
- name: Install asdf
  uses: ynab/asdf-action@v1.2
  with:
    version: 0.16.2
- name: Checkout code which includes a .tool-versions file in root
  uses: actions/checkout@v4
- name: Install asdf runtimes
  run: |
    asdf plugin add nodejs
    asdf install    
```
