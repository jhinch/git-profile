![CI](https://github.com/jhinch/git-profile/workflows/CI/badge.svg)

# `git-profile`

A git extension for managing multiple profiles which can be reused across repositories.

# Why

git currently provides 3 levels of configuration: the repository level, the user level
and system wide. When managing multiple personas (work vs personal, RL vs online), these
levels of configuration are too coarse grain, and managing completely different operating
system users just for git configuration can be painful. Luckily, git has an advanced
feature which allows for conditional includes in its configuration based on the directory
the repository is in. `git-profile` takes advantage of this and builds a profile
management system around it. A profile is simply a named git configuration file which can
be referenced.

## Usage

Before creating or configuring any profiles, you'll need to initialize `git profile`

    git profile init

This will create a `~/.git-profile` directory which will contain the profiles as well as
set up the relevant as well as a `.git-profile/.config` file which contains all the
`git-profile` configuration.

For more information see `git profile help`.
