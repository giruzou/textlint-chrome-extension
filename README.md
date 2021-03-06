# textlint Chrome Extension

[![wercker status](https://app.wercker.com/status/2f32f541de3ca03d8c8bc95152953ee9/s/master "wercker status")](https://app.wercker.com/project/bykey/2f32f541de3ca03d8c8bc95152953ee9) [![GitHub license](https://img.shields.io/github/license/io-monad/textlint-chrome-extension.svg)](LICENSE) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)

Chrome Extension that proofreads `<textarea>` using [textlint](http://textlint.github.io/).

## How to build

    $ npm install
    $ npm run build

To test the built extension, load `dist/chrome` directory into Chrome.

### Build for other browsers

:rocket: The extension experimentally supports Firefox ([WebExtensions](https://developer.mozilla.org/en-US/Add-ons/WebExtensions)) and Opera.

Check out [Experimental support for other browsers](docs/other-browsers.md) for more details.

## Tasks

### Watch build

Watch file changes and build it continuously.

    $ npm run watch

### Pack

Produce a production-packaged zip in `packages` directory.

    $ npm run pack

### Release

Versioning and release flow is automated by [semantic-release](https://github.com/semantic-release/semantic-release).

- For each push on `master` branch, [CI](https://app.wercker.com/project/bykey/2f32f541de3ca03d8c8bc95152953ee9) will execute semantic-release after all tests passed.
- Automatically determines the version of a release. `version` field in both `package.json` and `manifest.json` will be set at the release time.
- Automatically creates a git release with a release note that is auto-generated by commit messages.
- Automatically uploads a zip file to Chrome Web Store.

## Changelog

See [Releases](https://github.com/io-monad/textlint-chrome-extension/releases)

## License

This software is licensed under [GNU GPLv3](https://www.gnu.org/copyleft/gpl.html). See [LICENSE](LICENSE) for full text of the license.

Before version 2.0.0, this extension was licensed under The MIT License. Since this extension started to bundle some GPLv3 plugins, I decided to re-license the extension under GPLv3.
