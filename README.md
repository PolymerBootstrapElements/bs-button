# <bs-button>

Bootstrap Design for Buttons thru Polymer Components.

Buttons as defined in Bootstrap: http://getbootstrap.com/css/#buttons

## Installation

Using bower `npm install -g bower`

```
bower install --save PolymerBootstrapElements/bs-button
```

## Usage

For this bare Bootstrap code:

```html
<button class="btn btn-success btn-block active btn-lg">
    <span class="glyphicon glyphicon-globe"></span>
    Visit website
</button>
```

You get this using <bs-button>:

```html
<bs-button type="success" block active size="lg" icon="globe">
    Visit website
</bs-button>
```

All properties are bindable.

## API

### Properties

Name         | Type      | Default                 | Description
-------------|-----------|-------------------------|---------
**type**     | *String*  | `'default'`             | Button predefined style ([see](http://getbootstrap.com/css/#buttons-options))
**block**    | *Boolean* | `false`                 | Button as block
**disabled** | *Boolean* | `false`                 | Disabled state button
**size**     | *String*  | `undefined`             | Button predefined size ([see](http://getbootstrap.com/css/#buttons-sizes))
**icon**     | *String*  | `undefined`             | Glyph Icon to insert at button start ([see](http://getbootstrap.com/components/#glyphicons))
**href**     | *String*  | `'javascript:void(0);'` | `<bs-link-button>` only, anchor link url

Note: `<bs-link-button>` adds `href` property placed in `<a href={{href}}>`.

### Events

Name        | Data         | Description
------------|--------------|-----------
**click**   | -            | Raised when user click on button/link

## Contribution

1. Fork it

3. Code ^^

4. Create or update *./test* for each polymer component you modify.

5. Update demo page (*./demo/index.html*) and *README.md* if applicable

5. Create a PR and pray
