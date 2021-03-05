# config-stylelint

_config-stylelint_ is a configuration preset for [stylelint] used by the [fundamend.dev] ecosystem.

## Installation

Use your favorite Node.js package manager, for example [npm], like so:

    npm install --save-dev @fundamend/config-stylelint

... or [yarn], like so:

    yarn add --dev @fundamend/config-stylelint

## Usage

In your [.stylelintrc.js], import _config-stylelint_ and spread it into the exported object, like so:

```js
const fundamend = require('@fundamend/config-stylelint');

module.exports = {
	...fundamend,
};
```

You can extend the imported preset by adding additional [configuration options] to the exported configuration object, for example like this:

```js
const fundamend = require('@fundamend/config-stylelint');

module.exports = {
	...fundamend,
	rules: {
		'color-hex-case': 'upper',
	},
};
```

Settings that already exist in the configuration preset will be overwritten.

## License

[MIT]

[configuration options]: https://stylelint.io/user-guide/rules/list
[fundamend.dev]: https://fundamend.dev
[mit]: https://choosealicense.com/licenses/mit/
[npm]: https://www.npmjs.com/
[stylelint]: https://stylelint.io/
[.stylelintrc.js]: https://stylelint.io/user-guide/configure
[yarn]: https://yarnpkg.com/
