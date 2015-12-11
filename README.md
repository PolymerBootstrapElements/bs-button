# bs-button

[![Build Status](https://travis-ci.org/PolymerBootstrapElements/bs-button.svg?branch=master)](https://travis-ci.org/PolymerBootstrapElements/bs-button)

Bootstrap Design for Buttons thru Polymer Components.

Buttons as defined in Bootstrap: http://getbootstrap.com/css/#buttons

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Usage

Bootstrap should be referenced in your web page if you want to get benefits from &lt;bs-button&gt; element.

```html
<link rel="stylesheet" href="libs/bs/boostrap.css">
<script src="libs/bs/bootstrap.js"></script>
```

Use **bs-button** like this:

```html
<!-- Includes both bs-button and bs-link-button elements -->
<link rel="import" href="libs/bs-button/bs-button.html">

<bs-button type="success" block active size="lg" icon="globe">
    Visit website
</bs-button>
```

To generate this Bootstrap code:

```html
<button class="btn btn-success btn-block active btn-lg">
    <span class="glyphicon glyphicon-globe"></span>
    Visit website
</button>
```

## Development

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/bs-button/`, where `bs-button` is the name of the directory containing it.


## Test

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/bs-button/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.

## Contribution

1. Fork it
2. Code
3. Create or update [test suite](test/) for each polymer component you modify.
4. Update [demo page](demo/index.html) and [README.md](README.md) (this file) if applicable.
5. Create a PR and pray
