# material-design-iconfont

Bower package containing the [Material Icons](https://github.com/google/material-design-icons) icon font from Google.

This is a re-hosted copy of version `0.0.2` of [zckrs/material-design-iconfont](https://github.com/zckrs/material-design-iconfont) (upstream commit `b1000df0f486818b0dadcf360eb0989045a8cd20`), which is no longer available. The contents were restored from a local bower cache and are unchanged.

## Contents

```
iconfont/
├── MaterialIcons-Regular.eot
├── MaterialIcons-Regular.ttf
├── MaterialIcons-Regular.woff
├── MaterialIcons-Regular.woff2
├── codepoints      # icon name → unicode codepoint mapping
└── README.md       # Google's original usage note
```

## Installation

Add the dependency to your project's `bower.json`, pointing at this repository and tag:

```json
"dependencies": {
  "material-design-iconfont": "https://github.com/<account>/material-design-iconfont.git#~0.0.2"
}
```

Then run:

```bash
bower install
```

The package is installed to `bower_components/material-design-iconfont`, the same path as the original package, so existing build scripts keep working.

## Usage

Declare the font face, pointing at the installed font files:

```css
@font-face {
  font-family: 'Material Icons';
  font-style: normal;
  font-weight: 400;
  src: url(bower_components/material-design-iconfont/iconfont/MaterialIcons-Regular.eot);
  src: local('Material Icons'),
       local('MaterialIcons-Regular'),
       url(bower_components/material-design-iconfont/iconfont/MaterialIcons-Regular.woff2) format('woff2'),
       url(bower_components/material-design-iconfont/iconfont/MaterialIcons-Regular.woff) format('woff'),
       url(bower_components/material-design-iconfont/iconfont/MaterialIcons-Regular.ttf) format('truetype');
}

.material-icons {
  font-family: 'Material Icons';
  font-weight: normal;
  font-style: normal;
  font-size: 24px;
  line-height: 1;
  letter-spacing: normal;
  text-transform: none;
  display: inline-block;
  white-space: nowrap;
  word-wrap: normal;
  direction: ltr;
  -webkit-font-feature-settings: 'liga';
  -webkit-font-smoothing: antialiased;
}
```

Then use an icon by its name (see `iconfont/codepoints` for the full list):

```html
<i class="material-icons">delete</i>
```

## Versioning

Bower resolves versions from git tags. This repository has a single tag, `0.0.2`, which matches the original release. Don't move or delete it.

## License

- Package metadata: MIT, as declared by the original package.
- Font files: Material Icons by Google, licensed under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0).
