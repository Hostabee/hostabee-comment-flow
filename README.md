# \<hostabee-comment-flow\>

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![Build Status](https://travis-ci.org/Hostabee/hostabee-comment-flow.svg?branch=master)](https://travis-ci.org/Hostabee/hostabee-comment-flow) [![Greenkeeper badge](https://badges.greenkeeper.io/Hostabee/hostabee-comment-flow.svg)](https://greenkeeper.io/)

Commenting solution out-of-the-box in a web component.

```html
<hostabee-comment-flow></hostabee-comment-flow>
<script>
  const flow = document.querySelector('hostabee-comment-flow');
  // Populate the comment flow
  fetch('https://YOUR_API/comments')
    .then(res => res.json())
    .then(json => flow.comments = json.result);
</script>
```

![Screenshot of hostabee-comment-flow](https://raw.githubusercontent.com/Hostabee/hostabee-comment-flow/master/screenshot.png)

## Installation

Install `<hostabee-comment-flow>`:

```shell
bower install Hostabee/hostabee-comment-flow --save
```

Once installed, import it in your application:

```html
<link rel="import" href="bower_components/hostabee-comment-flow/hostabee-comment-flow.html">
```

### OPTIONAL

You can also install [exif-js](https://github.com/exif-js/exif-js) and [JavaScript-Load-Image](https://github.com/blueimp/JavaScript-Load-Image) to automatically fix [EXIF orientation on client-side](https://stackoverflow.com/questions/20600800). Be sure those 2 libraries are imported into your app before the `hostabee-comment-flow` element.

## Running demos and tests in a browser

1. Fork the `hostabee-comment-flow` repository and clone it locally.

2. Make sure you have [npm](https://www.npmjs.com/) and [Bower](https://bower.io) installed.

3. When in the `hostabee-comment-flow` directory, run `npm install` and then `bower install` to install dependencies.

    * [OPTIONAL] If you want to run tests or demo of the element involving the `hostabee-comment-flow-firebase-connector` you have to provide the configuration of your application in the _"test/firebase-config.js"_ and _"demo/firebase-config.js"_ files.

4. Run `npm start`, browser will automatically open the component API documentation.

5. You can also open demo or in-browser tests by adding **demo** or **test** to the URL, for example:

- http://127.0.0.1:3000/components/hostabee-comment-flow/demo/hostabee-comment-flow/basic.html
- http://127.0.0.1:3000/components/hostabee-comment-flow/test

## Running Tests

- When in the `hostabee-comment-flow` directory, run `polymer test`

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git cz` **OR** [follow this commit guide](https://conventionalcommits.org/) to write the commit messages.

4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request.

## License

Apache License 2.0
