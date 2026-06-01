# @wikytam/biome-config

My personal BiomeJS config for all projects.

## Install

```bash
pnpm i -D @wikytam/biome-config @biomejs/biome

#or npm
npm install -D @wikytam/biome-config @biomejs/biome
```

## Usage

In your project:

```json
{
  "$schema": "https://biomejs.dev/schemas/2.1.2/schema.json",
  "extends": ["@wikytam/biome-config"]
}
```

And finally, add the following scripts to your package.json to easily format and lint your code:

```json
{
  "scripts": {
    "format": "biome format --write .",
    "lint:ci": "biome ci .",
    "lint:fix": "biome check --write --unsafe .",
    "lint": "biome check .",
  }
}
## License

MIT
