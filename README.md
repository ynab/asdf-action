# asdf GitHub Action

GitHub Action that installs and configures [asdf](https://asdf-vm.com/) version >= 0.16.

This action supports Linux (AMD) and macOS (ARM) runners.

## Example usage

```yaml
- name: Install asdf
  uses: ynab/asdf-action@v1
  with:
    version: 0.16.2    
```
