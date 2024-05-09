cli-postgres
=================

A new CLI generated with oclif


[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/cli-postgres.svg)](https://npmjs.org/package/cli-postgres)
[![Downloads/week](https://img.shields.io/npm/dw/cli-postgres.svg)](https://npmjs.org/package/cli-postgres)


<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g cli-postgres
$ cli-postgres COMMAND
running command...
$ cli-postgres (--version)
cli-postgres/0.0.0 darwin-arm64 node-v20.12.2
$ cli-postgres --help [COMMAND]
USAGE
  $ cli-postgres COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`cli-postgres hello PERSON`](#cli-postgres-hello-person)
* [`cli-postgres hello world`](#cli-postgres-hello-world)
* [`cli-postgres help [COMMAND]`](#cli-postgres-help-command)
* [`cli-postgres plugins`](#cli-postgres-plugins)
* [`cli-postgres plugins add PLUGIN`](#cli-postgres-plugins-add-plugin)
* [`cli-postgres plugins:inspect PLUGIN...`](#cli-postgres-pluginsinspect-plugin)
* [`cli-postgres plugins install PLUGIN`](#cli-postgres-plugins-install-plugin)
* [`cli-postgres plugins link PATH`](#cli-postgres-plugins-link-path)
* [`cli-postgres plugins remove [PLUGIN]`](#cli-postgres-plugins-remove-plugin)
* [`cli-postgres plugins reset`](#cli-postgres-plugins-reset)
* [`cli-postgres plugins uninstall [PLUGIN]`](#cli-postgres-plugins-uninstall-plugin)
* [`cli-postgres plugins unlink [PLUGIN]`](#cli-postgres-plugins-unlink-plugin)
* [`cli-postgres plugins update`](#cli-postgres-plugins-update)

## `cli-postgres hello PERSON`

Say hello

```
USAGE
  $ cli-postgres hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ cli-postgres hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/letsdiscodev/cli-postgres/blob/v0.0.0/src/commands/hello/index.ts)_

## `cli-postgres hello world`

Say hello world

```
USAGE
  $ cli-postgres hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ cli-postgres hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/letsdiscodev/cli-postgres/blob/v0.0.0/src/commands/hello/world.ts)_

## `cli-postgres help [COMMAND]`

Display help for cli-postgres.

```
USAGE
  $ cli-postgres help [COMMAND...] [-n]

ARGUMENTS
  COMMAND...  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for cli-postgres.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.0.21/src/commands/help.ts)_

## `cli-postgres plugins`

List installed plugins.

```
USAGE
  $ cli-postgres plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ cli-postgres plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/index.ts)_

## `cli-postgres plugins add PLUGIN`

Installs a plugin into cli-postgres.

```
USAGE
  $ cli-postgres plugins add PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into cli-postgres.

  Uses bundled npm executable to install plugins into /Users/g/.local/share/cli-postgres

  Installation of a user-installed plugin will override a core plugin.

  Use the CLI_POSTGRES_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the CLI_POSTGRES_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ cli-postgres plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ cli-postgres plugins add myplugin

  Install a plugin from a github url.

    $ cli-postgres plugins add https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ cli-postgres plugins add someuser/someplugin
```

## `cli-postgres plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ cli-postgres plugins inspect PLUGIN...

ARGUMENTS
  PLUGIN...  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ cli-postgres plugins inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/inspect.ts)_

## `cli-postgres plugins install PLUGIN`

Installs a plugin into cli-postgres.

```
USAGE
  $ cli-postgres plugins install PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into cli-postgres.

  Uses bundled npm executable to install plugins into /Users/g/.local/share/cli-postgres

  Installation of a user-installed plugin will override a core plugin.

  Use the CLI_POSTGRES_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the CLI_POSTGRES_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ cli-postgres plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ cli-postgres plugins install myplugin

  Install a plugin from a github url.

    $ cli-postgres plugins install https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ cli-postgres plugins install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/install.ts)_

## `cli-postgres plugins link PATH`

Links a plugin into the CLI for development.

```
USAGE
  $ cli-postgres plugins link PATH [-h] [--install] [-v]

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ cli-postgres plugins link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/link.ts)_

## `cli-postgres plugins remove [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ cli-postgres plugins remove [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-postgres plugins unlink
  $ cli-postgres plugins remove

EXAMPLES
  $ cli-postgres plugins remove myplugin
```

## `cli-postgres plugins reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ cli-postgres plugins reset [--hard] [--reinstall]

FLAGS
  --hard       Delete node_modules and package manager related files in addition to uninstalling plugins.
  --reinstall  Reinstall all plugins after uninstalling.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/reset.ts)_

## `cli-postgres plugins uninstall [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ cli-postgres plugins uninstall [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-postgres plugins unlink
  $ cli-postgres plugins remove

EXAMPLES
  $ cli-postgres plugins uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/uninstall.ts)_

## `cli-postgres plugins unlink [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ cli-postgres plugins unlink [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ cli-postgres plugins unlink
  $ cli-postgres plugins remove

EXAMPLES
  $ cli-postgres plugins unlink myplugin
```

## `cli-postgres plugins update`

Update installed plugins.

```
USAGE
  $ cli-postgres plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.0.19/src/commands/plugins/update.ts)_
<!-- commandsstop -->
