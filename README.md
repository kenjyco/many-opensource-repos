many-opensource-repos
=====================

A collection of many open-source repos across many programming languages
organized in a shell script for easy mass-cloning and exploration.

The repos.sh file:

- Defines a bunch of sub-directories per language
- Defines bash arrays per language containing git repositories
- Defines the `clone-opensource` shell function to clone all the included repos
  to their respective sub-directories
- Defines shell functions matching `opensource-*-repos` (for each
  language/group) as navigation shortcuts to `cd` directly to the sub-directory
- Defines the `opensource-update-all` shell func to update all the cloned repos
    - Uses the
      [repos-update script](https://github.com/kenjyco/base/blob/master/bin/repos-update)
      defined in my [base repo](https://github.com/kenjyco/base)

Source the `repos.sh` file and use the shell functions defined in there.

```
% source ./repos.sh

% clone-opensource
```
If you have <https://github.com/kenjyco/base> setup and have the `repos-update`
script available, you can use the `opensource-update-all` shell func defined in
`repos.sh`

```
% source ./repos.sh; clone-opensource; opensource-update-all
```

Also feel free to check out [this
gist](https://gist.github.com/kenjyco/28664a963635d96e497d2b6caf7bcc70), a
historical timeline and collection of Wikipedia links for open-source
terms/concepts, programming languages, text/stream editing tools,
companies/organizations, and people behind them.
