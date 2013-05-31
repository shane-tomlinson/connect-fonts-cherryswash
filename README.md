# connect-fonts-cherryswash

Cherry Swash fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-cherryswash");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/cherryswash-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/cherryswash-bold,cherryswash-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* cherryswash-bold
* cherryswash-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/cherryswash-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin
* en

5. Set your CSS up to use the new font by using the "Cherry Swash" font-family.
```
    body {
      font-family: 'Cherry Swash', 'sans-serif', 'serif';
    }
```

## Font Info
Cherry Swash

* Copyright: Copyright (c) 2012, Natalia Kasatkina (kasatkinanataliya@gmail.com)
* Trademark: Please refer to the Copyright section for the font trademark attribution notices.
* Designer: Kasatkina Nataliya
* Vendor: Nataliya Kasatkina

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-cherryswash
* Repo: https://github.com/shane-tomlinson/connect-fonts-cherryswash

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* https://github.com/stomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 1.1 of the SIL Open Font License

  http://scripts.sil.org/OFL

