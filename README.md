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
