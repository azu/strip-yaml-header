# strip-yaml-header [![Build Status](https://travis-ci.org/azu/strip-yaml-header.svg)](https://travis-ci.org/azu/strip-yaml-header)

Strip yaml header form markdown.

## Installation

```
npm install strip-yaml-header
```

## Usage

```js
var strip = require("strip-yaml-header");
var markdown = "---\n" +
               "title: title\n" +
               "---\n" +
               "test";
var result = strip(markdown);
assert.equal(result, "\n" +
                    "\n" +
                    "\n" +
                    "test");
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

MIT
