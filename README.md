# Github Actions

This repository contains a collection of Github Actions that can be used in
your workflows.

Its separated in branches, each branch contains a different project type: rust,
...

## Usage

To use this you can add this repository as a remote to your project:

```bash
git remote add actions git@github.com:joshuachp/github-actions.git
```

Then you can fetch the branch you want to use and merge it into your project
with the `--allow-unrelated-histories` flag:

```bash
git fetch actions
git merge --allow-unrelated-histories actions/rust
```

When you want to update the actions you can just fetch the branch again and
merge it:

```bash
git fetch actions
git merge actions/rust
```

## Credits

This project was started from
[jonhoo/rust-ci-conf](https://github.com/jonhoo/rust-ci-conf)
