# Plugins Template Repository

## Overview

This repository provides a template for managing plugins with a standardized JSON schema. The schema ensures consistent and structured information about the plugins, making it easier to manage, update, and utilize them in various applications. Plugins can be stored here in their separate folders or in a different location that is publicly accessible.

## JSON Schema

The JSON schema defines the structure for the plugin information and includes the following sections:

### Info

The `info` section provides metadata about the plugin collection.

- **title** (string, required): The title of the plugin collection.
- **version** (string, required): The version of the plugin collection.
- **description** (string, optional): A brief description of the plugin collection.

### Plugins

The `plugins` section is an array of individual plugin objects. Each plugin object contains the following properties:

- **name** (string, required): The name of the plugin.
- **version** (string, required): The version of the plugin.
- **description** (string, required): A brief description of the plugin.
- **url** (string, required): The URL where the plugin can be accessed or downloaded.

## Example JSON

Below is an example JSON file that conforms to the schema:

```json
{
  "$schema": "./plugins.schema.json",
  "info": {
    "title": "My Plugin Collection",
    "version": "1.0.0",
    "description": "A collection of useful plugins for various applications."
  },
  "plugins": [
    {
      "name": "PluginOne",
      "version": "1.0.0",
      "description": "This is the first plugin.",
      "url": "https://example.com/pluginone"
    },
    {
      "name": "PluginTwo",
      "version": "2.0.0",
      "description": "This is the second plugin.",
      "url": "https://example.com/plugintwo"
    }
  ]
}
```
