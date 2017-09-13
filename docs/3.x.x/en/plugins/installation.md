# Plugin installation

Allows the developer to install a plugin, using the CLI.

## Basic usage

Considering you want to install a plugin named `content-manager` you can run the following command:
`$ strapi install content-manager`.

This supposed that this plugin is published on the npm registry as `strapi-plugin-content-manager`.

The command installs the plugin in the `node_modules` folder of your Strapi application, and then, move the plugin itself in the `./plugins` folder, so you can edit and version it.

## Development mode

In order to make contributors life easier, a command is dedicated to development mode:
`$ strapi install plugin-name --dev` (eg. `$ strapi install content-manager --dev`)

This command creates a symlink between the Strapi application and the plugin, which should have been previously installed globally (`$ npm link` or `$ npm install plugin-name -g`).
