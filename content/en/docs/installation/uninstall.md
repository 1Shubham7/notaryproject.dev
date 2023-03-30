---
title: Uninstall the notation CLI and its configuration
description: Uninstall the notation CLI, plugins, and configuration files
weight: 2
---

The `notation` CLI uses the following directories for its binaries and configuration files:

- `NOTATION_BIN` is the directory for the `notation` binary.
- `NOTATION_LIBEXEC` is the directory for other binaries, such as plugins, used by the `notation`.
- `NOTATION_CONFIG` is the directory for the configuration files, including trust stores and trust policies.

**IMPORTANT:** `notation` has default values for `NOTATION_BIN`, `NOTATION_LIBEXEC`, or `NOTATION_CONFIG`, but `notation` does not set those environment variables. These environment variables are optional, but if you wish to override the default values, you can set them to another value. For more details on each directory as well as the default location of those directories on each platform, see [Notation directory structure for system configuration]({{< ref "/docs/how-to/directory-structure" >}}).

## Remove the notation CLI

Delete the `NOTATION_BIN` directory to remove the `notation` binary.

## Remove the additional binaries

Delete the `NOTATION_LIBEXEC` directory to remove the additional binaries, including plugins.

## Remove the configuration files

**IMPORTANT:** `notation` automatically creates the `NOTATION_CONFIG` directory if it does not exist. If you remove the `NOTATION_CONFIG` directory, `notation` will recreate the directory the next time you run a command.

Delete the `NOTATION_CONFIG` directory to remove the configuration files.