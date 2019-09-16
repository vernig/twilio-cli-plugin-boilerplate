# twilio-cli plugin boilerplate

This is a boilerplate for a twilio-cli plugin (inspired by https://github.com/twilio/plugin-debugger comm)

# Configure 

To properly configure your plugin you need to change / customize: 
* [Name of the plugin in package.json](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/a332e137206105a730258ad12b3dc26866bb3f4e/package.json#L2)
* [`oclif.name` of the plugin](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/a332e137206105a730258ad12b3dc26866bb3f4e/package.json#L37) (in package.json)
*  Name of the file(s) / folder(s) implementing the command. This will be the actual name of the command. E.g. in this repo, [this file](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/master/src/commands/myplugin/mycommand.js) implements the command `twilio myplugin:mycommand`)


## Install (for dev pourpose)

To imnstall it use:

```
twilio plugin:link <plugin-folder>
```

## Unlink

To uninstall the plugin

```
twilio plugin:unlink <plugin-folder>
```
