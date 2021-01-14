# VTEX CLI Plugin Logs

Extend the `vtex` toolbelt!

## Developing

1. Clone `vtex/toolbelt` and follow the steps on the Contributing section.
2. Clone/Create a plugin with this template.
3. Change the template name under this project's `package.json`.
2. Run `yarn link` on this project.
3. Now run `vtex link @vtex/cli-plugin-logs` (or the new name) on the `vtex/toolbelt` project.
4. Run `yarn watch` on the `vtex/toolbelt`
5. Test the command on a VTEX IO app with `vtex-test hello`

For more information, read [Ocliff Docs](https://oclif.io/docs/introduction).

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
![npm](https://img.shields.io/npm/v/@vtex/cli-plugin-logs)

<!-- toc -->
* [VTEX CLI Plugin Logs](#vtex-cli-plugin-logs)
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @vtex/cli-plugin-logs
$ vtex COMMAND
running command...
$ vtex (-v|--version|version)
@vtex/cli-plugin-logs/0.0.1 linux-x64 node-v12.20.1
$ vtex --help [COMMAND]
USAGE
  $ vtex COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`vtex logs [APP]`](#vtex-logs-app)

## `vtex logs [APP]`

Show apps production logs

```
USAGE
  $ vtex logs [APP]

OPTIONS
  -a, --all      Show all logs from this account's apps
  -h, --help     show CLI help
  -p, --past     Show logs already seen from this account's apps
  -v, --verbose  Show debug level logs
  --trace        Ensure all requests to VTEX IO are traced

EXAMPLES
  vtex logs
  vtex logs appName
  vtex logs --all
  vtex logs appName --past
```

_See code: [build/commands/logs.ts](https://github.com/vtex/cli-plugin-logs/blob/v0.0.1/build/commands/logs.ts)_
<!-- commandsstop -->
