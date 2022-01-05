# Plugin Template

Use this repo as a template for creating Lando plugins.

## Steps

1. Copy this repo into your new plugin repo
2. Change the items marked CHANGEME to the name of this plugin in the following files:
    * docs/config.js
    * docs/README.md
    * .lando.yml
    * actions-lando-config.yml
    * plugin.yml
    * package.json
3. Add in your files or migrate the files from another plugin.
4. Add in your testing examples and add them to .github/workflows
5. Copy the docs config page into usage.md in the docs folder.
5. Remove these steps and alter the changeme text below.
5. PROFIT!


# Lando CHANGEME Plugin

The lando CHANGEME plugin service.

## Installation

```bash
# With npm
npm install @lando/CHANGEME

# With yarn
yarn add @lando/CHANGEME
```

## Issues, Questions and Support

If you have a question or would like some community support we recommend you [join us on Slack](https://launchpass.com/devwithlando). Note that this is the Slack community for [Lando](https://lando.dev) but we are more than happy to help with this module as well!

If you'd like to report a bug or submit a feature request then please [use the issue queue](https://github.com/lando/CHANGEME/issues/new/choose) in this repo.

## Changelog

We try to log all changes big and small in both [THE CHANGELOG](https://github.com/lando/CHANGEME/blob/main/CHANGELOG.md) and the [release notes](https://github.com/lando/CHANGEME/releases).


## Development

* Requires [Node 14+](https://nodejs.org/dist/latest-v14.x/)
* Prefers [Yarn](https://classic.yarnpkg.com/lang/en/docs/install)

```bash
git clone https://github.com/lando/CHANGEME.git && cd CHANGEME
yarn install
```

If you dont' want to install Node 14 or Yarn for whatever reason you can install [Lando](https://docs.lando.dev/basics/installation.html) and use that:

```bash
git clone https://github.com/lando/CHANGEME.git && cd CHANGEME
# Install deps and get node
lando start

# Run commands
lando node
lando yarn
```

## Testing

```bash
# Lint the code
yarn lint

# Run unit tests
yarn test
```

## Releasing

```bash
yarn release
```

## Contributors

<a href="https://github.com/lando/CHANGEME/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=lando/CHANGEME" />
</a>

Made with [contributors-img](https://contrib.rocks).

## Other Resources

* [Important advice](https://www.youtube.com/watch?v=WA4iX5D9Z64)