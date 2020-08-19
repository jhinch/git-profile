![CI](https://github.com/jhinch/git-profile/workflows/CI/badge.svg)

# `git-profile`

A git extension for managing multiple profiles. The extension is under active
development and is not currently ready for consumption.

## Future features

This is how it should work:

    # Initialize the configuration for git-profile
    git profile init

    # lists the current profiles
    git profile
    # or
    git profile list

    # Create a profile
    git profile add <profile-name>

    # Set the current profile
    git profile current <profile-name>
    # or using --subdirectory or --default

    # Get/Modify the configuration for a profile
    git profile config <profile-name> ...

## Principles for development

* Delegate and forward to the git binary where possible to avoid
  having to maintain feature parity with builtins
