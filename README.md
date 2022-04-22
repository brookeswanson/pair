## `pair`

When installed in a git repository, it appends the Co-authored strings of your pairs
to commit messages.

### Install

In a git repository run:

```shell
$ pair install
```

### Use

You can solo, remove a pair, or add a pair using the `pair` command:

```shell
$ pair
Looks like you're soloing.
You can:
[0] Add a pair
[1] Remove a pair
[2] Solo
```

Use the numbers for your selections and `q` when you are finished to exit.

Use jq to pull out the pair names for use in your shell prompt:

``` shell
jq -r '.pair_names|join(", ")' "$HOME/.pair-state.json"
```
