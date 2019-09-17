# twilio-cli plugin boilerplate

This is a boilerplate for a twilio-cli plugin (inspired by [plugin-debugger](https://github.com/twilio/plugin-debugger))

# Quick start

* Make sure `twilio-cli` is installed (follow instructions [here](https://www.twilio.com/docs/twilio-cli/quickstart#install-twilio-cli))
* Clone this repository
```
git clone https://github.com/vernig/twilio-cli-plugin-boilerplate.git
```
* _Link_ the plugin to your twilio CLI installation
```
twilio plugin:link <plugin-folder>
```
* Test it:
```
twilio twilio myplugin:mycommand
```
* If everything is set up cxorrectly you should see:
```
$ twilio myplugin:mycommand
Hello World!
```

# Configure 

To properly configure your plugin you need to change / customize: 
* [Name of the plugin in package.json](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/a332e137206105a730258ad12b3dc26866bb3f4e/package.json#L2)
* [`oclif.name` of the plugin](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/a332e137206105a730258ad12b3dc26866bb3f4e/package.json#L37) (in package.json)
*  Name of the file(s) / folder(s) implementing the command. This will be the actual name of the command. E.g. in this repo, [this file](https://github.com/vernig/twilio-cli-plugin-boilerplate/blob/master/src/commands/myplugin/mycommand.js) implements the command `twilio myplugin:mycommand`)

# Unlink

To _unlink_ the plugin

```
twilio plugin:unlink <plugin-folder>
```
