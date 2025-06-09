# carto-cjk

The original [carto](https://github.com/mapbox/carto) was last updated in 2020
and archived in 2024.

This repo is a drop-in replacement for Mapnik v4.0.6 and onward,
only adding a `lang` attribute to `TextSymbolizer`. This handles variation in
how a character is displayed in language contexts such as Simplified Chinese, Traditional Chinese, and Japanese (provided your font supports it).

You can set the attribute to an ISO language code (`zh-Hant`) or an expression (`[language]`) in env:

```javascript
let env = { lang: '[language]', ... };
new carto.Renderer(env, options)
```

## Authors of original Carto

* Tom MacWright (tmcw)
* Konstantin Käfer (kkaefer)
* AJ Ashton (ajashton)
* Dane Springmeyer (springmeyer)
* Michael Glanznig (nebulon42)
