
## Development

Install NPM dependencies with `yarn`.

To execute the tests, run `yarn test`.

For the best development experience, make sure that your editor supports [ESLint](https://eslint.org/docs/user-guide/integrations) and [EditorConfig](http://editorconfig.org).

Linting of code and commit message happens on commit via [Husky](https://github.com/typicode/husky).

## Releasing to NPM

Commit all changes and run the following:

```shell
$ npm login
$ yarn version --<update_type>
$ npm publish
```

… where `<update_type>` is one of `patch`, `minor`, or `major`. This will update the `package.json`, and create a tagged Git commit with the version number.

## Contributing

Pull requests are very welcome. Feel free to discuss bugs or new features by opening a new [issue](https://github.com/qqilihq/ecb-euro-exchange-rates/issues).

